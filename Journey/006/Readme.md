
![image](https://github.com/ericrihm/100DaysOfCloud/assets/19367455/7fdaee70-3511-4f4d-a636-8cbcfd03bc5b)


# AzureGoat: Insecure Object Reference (IDOR)

## Introduction

✍️ (Why) Explain in one or two sentences why you choose to do this project or cloud topic for your day's study.

## Use Case

- ✍️ (Show-Me) Explain in one or two sentences the use case

## Cloud Research
I created a test user and proceeded to change the password and check the payload sent

![image](https://github.com/ericrihm/100DaysOfCloud/assets/19367455/0b8725fc-fc90-4ab7-ac09-a023f34181ee)

- We can see there is a field id: "8" that may refer to the specific user

<br>I then fired up BurpSuite and used intercepter to capture this request. I then forwarded it to repeater to modify the ID field and see what response we get.
- At first I kept getting authetntication errors thinking this wasn't possible, but I changed the value back to the original and sitll got the same error.
After re-enabling intercepter and capturing the request possible I was able to successfully forward a password change for the user John Doe!

![image](https://github.com/ericrihm/100DaysOfCloud/assets/19367455/9c0171f0-ec1d-4fad-b0ff-69df60059a65)


## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)
