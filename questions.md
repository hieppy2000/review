# Write a script to find the second largest integer in a list not using python inbuilt functions like sorted
```
  - Input: l=[22,3,0,1,1111,1,45,78,8]
  - Output: return 78
```

# Print only repeated items which count more than 1
  ```
  - Input: 
      lines = 
      [ 'Eburger.letter.com - - [01/Jul/1995:00:00.15 -0400] "GET /shuttle/countdown/liftoff.html HTTP/1.0" 304 0',
        'Eburger.letter.com - - [01/Jul/1995:00:00.11 -0400] "GET /shuttle/countdown/liftoff.html HTTP/1.0" 304 0',
        'Eburger.letter.com - - [01/Jul/1995:00:00.11 -0400] "GET /shuttle/countdown/liftoff.html HTTP/1.0" 304 0',
        'Eburger.letter.com - - [01/Jul/1995:00:00.12 -0400] "GET /shuttle/countdown/liftoff.html HTTP/1.0" 304 0',
        'Eburger.letter.com - - [01/Jul/1995:00:00.12 -0400] "GET /shuttle/countdown/liftoff.html HTTP/1.0" 304 0']
  - Output:
        - Return this list = [
        01/Jul/1995:00:00.11 -0400,
        01/Jul/1995:00:00.12 -0400
        ]
  - Codes:
    lines = "\n".join(lines)

    new_lines = re.findall("\[.*\]", lines, re.MULTILINE)

    expected_line = ""

    #Print only occurrence more than 1
    outputs = list(set([x for x in new_lines if new_lines.count(x) > 1]))
    for output in outputs:
        print output.replace("[", "").replace("]", "")
  ```

# Return duplicated count item in a list:
```
- Input:
        l1 = ["a", "b", "c", "d", "a"]
- Output:
        a:2
        b:1
        c:1
        d:1
- Code:
    #trim duplicate item:
    trim_list_str = [] # ["a", "b", "c", "d"]
    for item in l1:
        if item not in trim_list_str:
            trim_list_str.append(item)

    for item in trim_list_str:
        print item + ":%d" %l1.count(item)
```
