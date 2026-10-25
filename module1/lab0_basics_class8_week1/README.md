# lab0_basics_class8_week1

In this lab homework we create three EC2 instances, making note of: 

* the IP address for the EC2
* connection method
* include a screenshot of the connection
* indicate if the instance was terminated

I have uploaded the screenshots to the screenshots folder in the GitHub repository.

| Deployment | IP address | Screenshot filename | Instance terminated |
| --- | --- | --- | --- |
| 1 | 18.117.167.47 | deployment-1.png | yes |
| 2 | 18.222.250.37 | deployment-2.png | yes |
| 3 | 13.184.17.200 | deployment-3.png | yes |

Additional information:

During the first deployment, I confirmed the template was available to use and pasted the script into the templates's User data field. I then connected to the instance using SSH. From there I ran the command "seir-dashboard". I had to redo this instance because I did not capture the correct output.

On the second deployment, I still had to adjust the template. This time I connected to the webiste instead of SSH. I got the output and updated this README.md file.

For the third deployment, I did what I did for the second one, but it was a little faster process this time. I did not leave either running to see an impact on the computer performance.
