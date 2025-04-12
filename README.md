This is my personal script that I've been using in my current setup. I've been trying to make this work with the built-in CURL command of AgentDVR but it just doesn't. Luckily, AgentDVR has a feature where one can add their own bash/bat script to run a command. You don't need a subscription to make this work.

# How to make this work?

1. Instruction for the script are in the script.
2. Copy the file inside AgentDVR/Commands/
3. Open AgentDVR Web UI
4. Edit the IPCam you want to have this command.
5. Navigate to Actions > Add > Task
6. Under Task, Choose Execute Command
7. With File, choose the filename you chose for the file in 2.
8. Under Parameters, add these: {0:H:mm:ss} {AI} {BASE64IMAGE} {NAME} then click OK
   * These parameters corresponds to the tags in the script with $1, $2 etc..
9. Under If, if you want to test, you can choose Manual Alert, in my case, I'm choosing AI: Object Found
10. OK, then OK.

## DISCLAIMER: I DON'T THINK THERE WILL BE ANY UPDATE TO THIS.
