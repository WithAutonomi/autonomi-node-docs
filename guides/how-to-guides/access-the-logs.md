---
description: >-
  If you're interested, or asked to, here's how to access the logs of the nodes
  running on your machine when you are using the Node Launchpad
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/mHMagc6BlRPNTxTKcyjL/guides/how-to-guides/access-the-logs
---

# Access the Logs

## To Access the Logs for each of your Nodes

{% stepper %}
{% step %}
In the Node Launchpad **Press O** to open the Options screen.
{% endstep %}

{% step %}
Press **Ctrl + L.** This will open the folder which contains all the log files for each node on your device.
{% endstep %}

{% step %}
Open the directory for the node you want to take a look at then open the 📁 **logs** folder. Inside you'll find the latest log file named **`antnode.log`**

You can open this to take a peek at the logs themselves, or forward it on to the support team if you need to.
{% endstep %}
{% endstepper %}



## To Access the Launchpad's Logs

The launchpad app itself also keeps logs. These are useful to access when the app crashes, or has other problems, and will help us fix and improve the experience. So if you are asked to provide these by a member of the team, here's how to do that



<details>

<summary>Accessing the Launchpad logs in <strong>Windows</strong></summary>

1. **Open File explorer**
2.  **Select the View tab**, then select **Hidden Items checkbox**  as shown below\
    <br>

    <figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeTIykFbRzUzyGABRujAQjLSUDbjCKUfTz9uC3IKfZb9gF5URGfzKZbrBvT-RojxJDRDrUnThCrmZ_KiQKOU-AimIits0yLVP_uzvl4NvadKx0lLd_9Uwfm9uiZXFgh5_F-ZM467Q_BseM_e51nQYQzlptb?key=sGrzvkGPpvvdENaW6TnLbw" alt=""><figcaption></figcaption></figure>
3. Navigate to **%AppData%\autonomi\launchpad\logs**

You'll find the Launchpad logs in this folder. The last one created around the time when a crash or issue occurred will be the most useful.

</details>

<details>

<summary>Accessing the Launchpad logs in <strong>Mac</strong></summary>

1. **Open the Finder**
2. **Click Go** in the task bar at the top of your screen
3. While Holding down the **Option ⌥** key click the **🏛️ Library** menu item that appears&#x20;
4. Navigate to **📁 Application Support > 📁 autonomi > 📁 launchpad > 📁 logs**&#x20;

You'll find the Launchpad logs in this folder. The last one created around the time when a crash or issue occurred will be the most useful.

</details>

<details>

<summary>Accessing the Launchpad logs in <strong>Linux</strong></summary>

You'll find the logs in the following location:\
\
`~/.local/share/autonomi/launchpad`\
\
The last log file one created around the time when a crash or issue occurred will be the most useful.

</details>
