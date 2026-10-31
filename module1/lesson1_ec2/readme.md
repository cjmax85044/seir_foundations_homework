## Week 3 Homework

*Every screenshot in this HW must show the ID line: whoami && TZ='Your/Zone' date && ec2-metadata -i && uptime -s*

### Lab Requirements:
- Each run = one brand-new EC2 instance, Steps 0–4 completed by hand
- Run the ID line right before starting uvicorn. The screenshot must show the ID line output and "Application startup complete."
- Max 3 lab-run screenshots per day (your local time), so you need at least 3 separate days
- List all 7 runs in a .md table in your lesson1_ec2 README.md
- Upload personal notes as "lab1_notes.md"
- Terminate every instance after each run and check for leftover volumes / Elastic IPs

### COBOL Core Practice:
- Every TXN ID you post must start with your initials
- Trigger every return code on purpose, then run echo $?
- Decode the fixed-width ledger by hand using cut -c
- Add a "COBOL practice" section to lab1_notes.md


LAB RESULTS
| Run | Date | Time Zone | Instance ID | Boot time (UTC) | Public IPv4 DNS | Screenshot | Terminated|
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 10/30/26 | MDT | i-0626a190ca3afa79f | 17:12 | 54.159.21.75 | yes | coreybank1_10-30-26_35.172.185.243_lab_screenshot.png |
| 2 | 10/30/26 | MDT | i-087e7195314094918 | 22:50 | 18.232.150.228 | yes | coreybank2_10-30-26_18.232.150.228_lab_screenshot.png |
| 3 | 10/30/26 | MDT | i-04f0d84fc9e728bb8 | 23:30 | 54.197.37.45 | yes | coreybank2_10-30-26_54.197.37.45_lab_screenshot.png |

All screenshots in the lesson1_3c2/screenshots directory.
