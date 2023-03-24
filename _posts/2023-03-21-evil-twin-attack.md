---
title: Evil Twin Attack
date: 2023-03-21 11:40:00 -500
image: https://i.postimg.cc/CKqnQtfp/evil-twin-02.jpg
categories: [Security, Cybersecurity]
tags: [hacking, wifi, network, vpn, https]
---

Let's talk a little on *cybersecurity*
### Introduction
---

Evil Twin Attack is attack is frequently carried our on wireless access points with malicious intentions.

---

This attack happens when attackers exploits a fundamental issue with Wi-Fi. That is, our Laptops, smartphones, and connected devices aren't equipped to distinguish between two radios broadcasting the same SSID name. This allows hackers to use malicious access points (APs) that eavesdrop (spy) on traffic, establish "man-in-the-middle" (MitM) positions, and extract sensitive information, often without leaving any traces behind.

![evil-twin-attack-01.png](https://i.postimg.cc/KvJVspnz/evil-twin-attack-01.png)

>>>>>> image source: okta .com

In a normal Wi-Fi connection, a person's client device (victim)) associates with a legitimate AP (on the right). When an evil twin AP is present, a threat actor broadcasts the same SSID as the legitimate AP (and often the same BSSID or MAC address of the SSID) to fool the device into connecting to the fake access point (on the left).
From the image, you can see that after the attack is successfully executed, the victim's internet connection now passes instead through the fake access point instead of the legitimate one.

### Explaining with a none tech example
---
What has been written above might be difficult for those who don't understand much of this technology stuff. 

Here, on PC Drills, we're there to help those who aren't experts to be able to understand.

Consider something like this;
> You have a particular radio station that you always listen to. Consider that, you don't know it's frequency mudulation (something like 110.2 FM but you don't know), all you know is the name of the radio station (maybe it's something like 'PC Drills Radio').

So, what you rely on to know you are listening to the correct radio station is when they say the name. Given that names are not unique (many stations can have the same name), another person who wants to impersonate the legitimate radio station can create their own radio station (maybe 108.1 FM) but still call it "PC Drills Radio".

How do you differentiate? Given you don't know their different frequencies, just like two people with different firstname but same last name, you can't differentiate from the last name.

In this example you can see that while tuning your radio, you might even reach the wrong radio station first, because it's closer to you (108.1 < 110.2). sometimes, because the signal is stronger and so on, will also determine which one you get.
That's the same thing that's happening in this kind of attack, your phone is connecting to the name, but no way to know if the name is the real one or counterfeit or dublicate or something else.


### What can you do to prevent Evil Twin AP attacks?
---

Businesses offering Wi-Fi to their employees and customers can use wireless intrusion prevention systems (WIPS) to detect the presence of an evil twin AP and prevent any managed corporate clients from connecting to them. You should also protect access points through the use of a Personal Security Key (PSK) and provide it to employees and customers.

End Users:

BUT for normal Wi-Fi users, an evil twin AP is nearly impossible to detect because the SSID appears legitimate and the attackers typically provide Internet service. In most cases, the best way to stay safe on unfamiliar Wi-Fi networks is to always use a VPN to encapsulate the Wi-Fi session in another layer of security.

### Avoiding Evil Twin Attacks
---

You can still follow these best practices:

1.   Avoid public free WiFi access altogether.
2.   Do not connect to open WiFi access points without verifying it as legitimate.
3.   Disable to auto connect feature and promiscuous mode on all wireless devices.
4.   Ask the establishment for the official name of their hotspot, and any security key if one exists. Intentionally type in the wrong key. Some evil twins will grant access to the hotspot no matter what key is entered.
5.   Don’t log into any accounts on public Wi-Fi. This way, the hacker will not be able to steal your credentials and use them against you.
6.   Avoid connecting to Wi-Fi hotspots that say ‘Unsecure,’ even if it has a familiar name.
7.   Use 2-factor-authentication for all your sensitive accounts. This way, even if a hacker gets hold of your login credentials, they will still struggle to get into your accounts.
8.   Learn to recognize social engineering attacks, phishing, and spoofed URLs.
9.   Only visit HTTPs websites, especially when on open networks. HTTPs websites provide end-to-end encryption, making it difficult or impossible for hackers to see what you do when you visit them.
10.   Don’t dismiss your device's notifications, especially if you were kicked off the network and you’re connecting to what you think is a known Wi-Fi network. If your device recognizes it as a new network, don’t ignore it!
11.   Don’t autosave Wi-Fi on your device because when it’s not connected to your home or office networks, it will transmit so-called probes. They can give out a lot of information about you, including your home address. Hackers can sniff this information and pretend to be your home network.
12.   Use a VPN whenever you connect to a public hotspot. It will encrypt your traffic before it leaves your device, making sure that no one sniffing the traffic can see your browsing behaviors.
_______

---
### Abreviations used
AP - Access Point

VPN - Virtual Private Network

BSSID - Network Mac Address Value (unique value)

SSID - Network Name

---
To get more updates. 
We're available on 
Facebook and Telegram.

Follow | [Telegram Channel](https://t.me/pcdrills/) | [Facebook Page](https://facebook.com/pcdrillsofficial/)

See you around
