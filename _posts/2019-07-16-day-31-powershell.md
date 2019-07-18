---
layout: post
title: "Day 31: Windows PowerShell"
date: 2019-07-16
---

**Today's Progress:** I spent the majority of my work day today working with Windows PowerShell in an attempt to get information about a bunch of folders on my company's shared drive. I wanted to find out the number of files in every folder (without counting the folders within the folders) and then export the data to a CSV file. I found a [discussion on idera.com](https://community.idera.com/database-tools/powershell/ask_the_experts/f/powershell_for_windows-12/7687/should-be-simple-recursive-file-count) that gave some code to get me started. This is the original code:

```powershell
PS> dir $env:windir -ea 0 -rec | Where-Object { $_.PSIsContainer } | Foreach-Object { $rv = 1 | Select-Object Path, Count; $rv.Path = $_.FullName; $rv.Count = Dir $_.FullName | Measure-Object -property Length -ea 0 | Select-Object -expandProperty Count; $rv }
```

I removed the `$env:windir` because I only wanted to count the files in the directory PowerShell was in and its subdirectories.

To export the data, I added the following code to the end of the above code, where `<string>` is the path to where I saved the file:

```powershell
| Export-Csv -Path <string> -NoTypeInformation -Append
```

The final code:

```powershell
dir -ea 0 -rec | Where-Object { $_.PSIsContainer } | Foreach-Object { $rv = 1 | Select-Object Path, Count; $rv.Path = $_.FullName; $rv.Count = Dir $_.FullName | Measure-Object -property Length -ea 0 | Select-Object -expandProperty Count; $rv } | Export-Csv -Path <string> -NoTypeInformation -Append
```

This works just as I want it to!

**Thoughts:** This isn't web development, but it's still coding. I used many of the same skills researching code and testing it out. I still had to use code-think!

**Links to today's work:** No links today
