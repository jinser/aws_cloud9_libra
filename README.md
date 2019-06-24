# Setting up Libra in AWS Cloud9 IDE

This is a short 3-step setup of a cloud-based IDE on AWS to start playing with the Libra code and test net. 



## 1. Creating the Cloud9 Environment

After some trial and error, the minimum memory required should be 2GB and the minimum disk space required is about 20G.
For this setup, Ubuntu is used instead of Amazon Linux.

Check out the screenshot below for which fields were selected for this guide:

![Screenshot](https://raw.github.com/jinser/aws_cloud9_libra/master/libra_cloud9_createenv.png)


## 2. Increasing disk space

The default disk space provided is 10G in cloud9, to increase the size, the resize.sh file provided here will have to be uploaded directly to the Cloud9 environment.
Once the upload is completed, run the following command in the same location as where the resize.sh file has been uploaded to:
```
`sh resize.sh 20`
```

![Screenshot](https://raw.github.com/jinser/aws_cloud9_libra/master/libra_cloud9_increase_diskspace.png)


If Amazon Linux is used, refer to the *Resizing an Environment* section of the [AWS official guide](https://docs.aws.amazon.com/cloud9/latest/user-guide/move-environment.html) instead.



## 3. Running through the Libra tutorial

And that is all to getting the Cloud9 IDE ready for starting with Libra!

Run through the [Libra tutorial setup](https://developers.libra.org/docs/my-first-transaction#steps-to-submit-a-transaction) with this environment to see the same success with connecting to the Libra testnet:

![Screenshot](https://raw.github.com/jinser/aws_cloud9_libra/master/libra_cloud9_success.png)
