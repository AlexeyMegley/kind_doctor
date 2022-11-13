# kind_doctor
Service for dermatology patients, helping with treatment and disease monitoring at home

# **Service goal**

Imagine the next situation:

Patient goes to a dermatologist and gets treatment instructions.<br>
After while patient reports the treatment has no effect and heads to hospital.<br>
In the hospital the patients has the same treatment and surprisingly the effect is great.<br>

#### What's the trick?

In the most these cases, patients take their drugs incorrectly.

It can be:
- irregular treatment (for example, patient forgets to take a pill several times during week)
- inadequate procedure (for example, "apply medicine to the skin" can be performed for 1 ml of medicine or for 10 ml of medicine etc.)
- wrong medicine was bought or the dosage is wrong
- and many other reasons

So, the main goal of the service is to decrease frequency of errors like these.


# **MVP**

At the end of appointment, doctor gives the patient name of bot + identifier used for authentication or link, that will be used to start the interaction with system. After "/start" command, patient gets pictures of medicines and additional prepared instructions (for example, link to youtube video, which shows how to apply medicine to the skin). After this patient can set up notification time + start the treatment. Starting from this period there will be "it's time to take a medicine" notifications + patient will need to take a picture of the affected area of the skin.

This picture will be preprocessed:
- Anonymizing (the eyes will be blurred, etc)
- It'll be checked the affected area is visible on the picture
- It'll be checked the brightness of the picture is sufficient

After that the picture will be saved at the server and can be used for progress tracking.

### **Improvement 1**
- Find patients, where there is no clear progress based on pictures and additionally notify doctor about these patients.

### **Improvement 2**
- Having image uploaded, choose additional questions to be asked and save answers for them also.


