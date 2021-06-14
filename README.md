# Demultiplexing-sequencing-by-HaplotypR-through-Docker

This is an example of demultiplexing:

1. Install and open an account with Docker

2. Go to lerch-a/HaplotypR (https://github.com/lerch-a/HaplotypR) and from here go to Docker image link (https://github.com/colbyford/HaplotypR-Docker)

3. Pull the Image to Local Machine and run locally as it is stated in there (it takes sometime to be completed)

4. Now be can see the image "haplotypR" is running in our Docker dashboard

5. Type "docker container ls" in terminal and under container ID we will have a specific alpha-numeric 12 digits, e.g. "9690b3181e68" 

6. Now we need to copy from my local machine (the given examples that I will use in my container) by "Copy File to Container" as "docker cp myfile.txt haplotypr:./myfile.txt". From lerch-a/HaplotypR it is the file "exdata" inside of "inst" file. In my given example is going to be as this:
	First go to my downloads by "cd Downloads" where my example folder is, and then type "docker cp HaplotypR-			master/. 9690b3181e68:/home/rstudio"

7. Now we are good to go! in Docker dashboard, at the  "haplotypR" image, click "open in a new browser"

8. From the lerch-a/HaplotypR (https://github.com/lerch-a/HaplotypR) copy and paste all the code since "Run HaplotypR on R command line" and run it, it will take some time (skip the installation process because we have now all the packages that are needed; in a compiled form by Docker)

