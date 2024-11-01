# Summary of IoMT Device Attack Impact and Security Research

- Various IoMT devices were tested for vulnerability against attacks.
- **Affected Devices**: Livlov Heart Rate Sensor, Wellue O2 Ring, Checkme BP2A,
  Rhythm+ 2.0, Lookee O2 Ring.
- **Unaffected Devices**: Wellue Pulsebit EX, Checkme O2 Smart Wrist Pulse
  Oximeter, SleepU Sleep Oxygen Monitor.
- A benchmark dataset (CICIoMT2024) was created to evaluate IoMT security
  solutions.
- The study highlights the need for robust cybersecurity measures in healthcare
  IoT applications to prevent data breaches and ensure patient safety.

What types of attacks were executed on the IoMT testbed in the research?

The research executed 18 types of attacks on the IoMT testbed, categorized into
five classes: 

1. **DDoS (Distributed Denial of Service)**
2. **DoS (Denial of Service)**
3. **Recon (Reconnaissance)**
4. **MQTT (Message Queuing Telemetry Transport) attacks**
5. **Spoofing**

What is the purpose of the CICIoMT2024 dataset created in the study?

The purpose of the CICIoMT2024 dataset is to provide a comprehensive and
realistic multi-protocol benchmark for assessing the security of Internet of
Medical Things (IoMT) devices. It aims to address existing gaps in IoMT security
research by including a diverse set of devices, a wide range of cyberattacks,
and detailed profiling of device behavior to aid in the development and
evaluation of security solutions in healthcare.

What is the purpose of the CICIoMT2024 dataset?

The purpose of the CICIoMT2024 dataset is to serve as a comprehensive benchmark
for assessing the security of Internet of Medical Things (IoMT) devices. It aims
to address gaps in existing datasets by including a diverse range of devices,
various cyberattacks, and detailed behavioral profiling, thereby aiding
researchers in developing and evaluating IoMT security solutions in healthcare.

What are some of the monitoring technologies mentioned in the context of IoMT
devices?

Some of the monitoring technologies mentioned in the context of IoMT devices
include:

1. **Heart rate and cardiovascular solutions** for tracking parameters like pulse rate, blood pressure, and oxygen saturation.
2. **Electrocardiogram (ECG) monitoring devices** for detecting anomalies in heart rhythms.
3. **Sleep and oxygen assessment technologies** for evaluating sleep patterns and blood oxygen levels.

How many real and simulated devices were used in the CICIoMT2024 dataset?

The CICIoMT2024 dataset used a total of 40 IoMT devices, comprising 25 real
devices and 15 simulated devices.

What are the main categories of attacks included in the dataset?

The main categories of attacks included in the CICIoMT2024 dataset are:

1. **DoS (Denial of Service)**
2. **DDoS (Distributed Denial of Service)**
3. **Spoofing**
4. **Recon (Reconnaissance)**
5. **MQTT (Message Queuing Telemetry Transport) attacks**

How does this dataset can help us to any further and future performance evaluation?

The CICIoMT2024 dataset can aid in future performance evaluation by providing a
realistic and diverse set of IoMT device behaviors and attack scenarios,
allowing researchers to benchmark and optimize machine learning algorithms for
detecting and mitigating cyber threats. It facilitates the exploration of new
features and hyperparameter tuning, enhancing the understanding of security
principles in healthcare. Additionally, the dataset's comprehensive nature
supports the development of more robust and effective security solutions for
IoMT environments.

What is meaning of profiling?

Profiling refers to the process of capturing and analyzing the behavior and
characteristics of devices or systems over time, particularly in terms of their
operational patterns and interactions within a network. In the context of IoMT,
profiling helps identify expected benign behaviors, enabling the detection of
anomalies and potential security vulnerabilities. This understanding is crucial
for enhancing the security and reliability of IoMT systems.

What are 18 different cyberattacks over diverse set of 40 IoMT devices?

The 18 different cyberattacks executed over the diverse set of 40 IoMT devices
include:

1. **DoS TCP**
2. **DoS ICMP**
3. **DoS SYN**
4. **DoS UDP**
5. **DDoS TCP**
6. **DDoS ICMP**
7. **DDoS SYN**
8. **DDoS UDP**
9. **MQTT Malformed Data**
10. **MQTT DoS Connect flood**
11. **MQTT DoS Publish flood**
12. **MQTT DDoS Connect flood**
13. **MQTT DDoS Publish flood**
14. **ARP Spoofing (Man-in-the-Middle)**
15. **Recon attacks**
16. **Spoofing attacks**
17. **Flooding campaigns (various types)**
18. **Other targeted attacks specific to IoMT protocols**

Why they have a lot of effort to develop comprehensive IoMT security dataset and
named it CICIoMT for developers or any medical IoMT device producers? 

The effort to develop the comprehensive IoMT security dataset, named
CICIoMT2024, aims to address existing gaps in IoMT security research by
providing a realistic benchmark for evaluating and developing security
solutions. It offers a diverse range of device behaviors, attack scenarios, and
protocols, which are essential for researchers and developers to create
effective cybersecurity measures tailored to the unique challenges of healthcare
environments. This dataset ultimately supports the advancement of secure IoMT
device deployment, ensuring the confidentiality, integrity, and availability of
medical services.

Can you tell me about attack scenarios and attack protocols?

Attack scenarios refer to specific situations or methods in which cyberattacks
are executed against IoMT devices, illustrating how attackers might exploit
vulnerabilities. Examples include Distributed Denial of Service (DDoS) attacks,
where multiple compromised devices overwhelm a target, or Man-in-the-Middle
attacks, where an attacker intercepts communication between devices.

Attack protocols are the communication standards or methods used during these
attacks, such as MQTT (Message Queuing Telemetry Transport) for messaging in
IoMT environments, TCP/IP for network communication, or ARP (Address Resolution
Protocol) for local network interactions. Understanding both scenarios and
protocols is crucial for developing effective security measures against
potential threats in IoMT systems.

What is the main motivation of this research?

The main motivation of this research is to address the limitations of existing
datasets and networking data processing pipelines in the context of medical
security, specifically for IoMT devices. By creating a realistic benchmark
dataset, the research aims to enable the development and evaluation of effective
IoMT security solutions, enhancing the overall cybersecurity posture of
healthcare systems. This effort seeks to support researchers in investigating
new mechanisms and improving the security of IoMT operations against various
cyber threats.

## Notes:

The complexity and data volume of IoMT network traffic requires advance methods
to enhance security and reliability.

Machine Learning offers techniques to detect, prevent, and mitigate
cyberattacks.

## Gaps

Existing benchmark datasets lack essential features for robust iomt security
solutions, such as reduced number of real devices, a limited variety of attack,
and a lack of extensive profiling.

## Protocols

+ Wi-Fi
+ MQTT
+ Bluetooth

## As their goal

1. Aiding researchers in creating secure heAlthcare systems using ML.
2. Beyond simulating attacks, we capture the lifecycle of IoMT devices from
network entry to exit through profiling, allowing classifiers to identify device
anomalies.
3. Their results as CICIoMT2024 release into CI dataset page, demonstrates that
various methods can classify IoMT cyberattacks.

## Importance of IoMT

IoT devices present a limited pool of computational resources compared to
traditional systems. This is a key factor to observe in terms of the device
security, their simpler network profiles these components bring to the network
(limited pool of protocols), and the possible open doors for attackers.

For instance, iot devices can be exploited in Advanced Persistent Threats (APT)
as key vectors. there is a current lack of standards for iot devices. for
example, the NIST maintains a repo for the vulnerability management of several
devices called the National Vulnerability Database (NVD). [nvd ref](https://nvd.nist.gov/).

Vulnerabilities discovered that can affect devices in use are shared in this
database to enable the general public to be aware and patch their systems. In
iot, devices are diverse and present multiple brands, firmware, and purposes.

Although there are some initiatives to create standard repo for iot, this
diversity makes it difficult for vulnerabilities to be tracked and patched for
all devices.

The main issue refers to the increase of iot as an important asset in many envs
as well as a main target for attackers.

All of theses benefits and cybersecurity concerns also apply to healthcare
applications. 

Some iot devices are not widely adopted in specific envs for instance, infusion
pumps are devices adopted in healthcare and unavailable in other envs
vulnerabilities.

For example, iot devices have been targeted in many ransomware attacks against
healthcare orgs in the past few years. In fact, security solutions need to
consider this aspect to different area of healthcare.

+ In terms of confidentiality, sensitive patient's information may be disclosed.
+ In terms of integrity, vital readings can be manipulated to compromise the
accuracy of the treatments provided.
+ In terms of availability, attacks may disrupt critical services and lead the
operations to un safe states.

In the context of IoMT, the primary security concerns comprise Confidentiality,
Integrity, and Availability (CIA) of safety critical applications.

Given the complexity and amount of data generated by iot and iomt network
traffic, advanced methods have become especially useful in these envs. In this
context, ML brings various techniques and solutions that can improve the
detection, prevention, and mitigation of cyber-attacks.

By analyzing the networking patterns in a multidimensional space, ML can
identify anomalies in the network, abnormal iomt traffic, and characteristics of
attacks that can be launched (DDoS).

ML can enable the automated detection of potential threats and help healthcare
professionals deliver high-quality services with a continuous security
monitoring approach.

A temp sensor can be implemented to send temp readings once a day. At the same
time, an aircraft sensor can be implemented to send structural readings
regularly. Alongside the temporal differences, iot services can also rely on
multiple protocols like MQTT, which can include specific patterns in the network
traffic.

Similarly, IoMT devices can operate differently depending on the app. for
example the traffic generated by an infusion pump is usually less frequent than
continuous physiological monitor. These differences can be learned or captured
by ML techniques to identify if abnormal traffic is sent through the network.

CICDataset contains some data. What's these data? Is it a bunch of data about
some medical devices network traffic to learn anomaly or noises data?

Although there are some datasets available for the development of security apps
in iomt, there are important features not addressed in the current
state-of-the-art contributions. for example operational diversity is a critical
aspect to consider to mimic a realistic iomt environment.