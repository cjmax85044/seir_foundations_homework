## Week 3 Homework

*Every screenshot in this HW must show the ID line: whoami && TZ='Your/Zone' date && ec2-metadata -i && uptime -s*

### Lab Requirements:
- Each run = one brand-new EC2 instance, Steps 0–4 completed by hand
- Run the ID line right before starting uvicorn. The screenshot must show the ID line output and "Application startup complete."
- Max 3 lab-run screenshots per day (your local time), so you need at least 3 separate days
- List all 7 runs in a .md table in your lesson1_ec2 README.md
- Upload personal notes as "lab1_notes.md"
- Terminate every instance after each run and check for leftover volumes / Elastic IPs


LAB RESULTS
| Run | Date | Time Zone | Instance ID | Boot time (UTC) | Public IPv4 DNS | Screenshot | Terminated|
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 10/30/26 | MDT | i-0626a190ca3afa79f | 17:12 | 54.159.21.75 | coreybank1_10-30-26_35.172.185.243_lab_screenshot.png | yes |
| 2 | 10/30/26 | MDT | i-087e7195314094918 | 22:50 | 18.232.150.228 |  coreybank2_10-30-26_18.232.150.228_lab_screenshot.png | yes |
| 3 | 10/30/26 | MDT | i-04f0d84fc9e728bb8 | 23:30 | 54.197.37.45 |  coreybank3_10-30-26_54.197.37.45_lab_screenshot.png | yes |
| 4 | 10/31/26 | MDT | i-0c35029f2c0db6e1a | 15:20 | 100.53.186.177 |  coreybank4_10-30-26_100.53.186.177_lab_screenshot.png | yes |
| 5 | 10/31/26 | MDT | i-06f521563ecfb17e9 | 16:00 | 54.227.71.59 |  coreybank5_10-31-26_54.227.71.59_lab_screenshot.png | yes |
| 6 | 10/31/26 | MDT | i-0d8628f0d4d9c6b34 | 16:48 | 13.220.113.100 | coreybank6_10-31-26_13.220.113.100_lab_screenshot.png | yes |
| 7 | 11/1/26 | MDT | i-08cd879a265691f06 | 8:30 | 54.211.102.30 | coreybank7_10-31-26_54.211.102.39_lab_screenshot.png | yes |

### COBOL Core Practice:
- Every TXN ID you post must start with your initials
- Trigger every return code on purpose, then run echo $?
- Decode the fixed-width ledger by hand using cut -c
- Add a "COBOL practice" section to lab1_notes.md

I used the seventh lab run for the COBOL practice


All screenshots in the lesson1_3c2/screenshots directory.
