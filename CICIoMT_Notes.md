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

To mimic a healthcare iomt infrastructure, a topology needs rely on the use of
multiple services that would naturally adopt different protocols (Wi-Fi,
Bluetooth, and MQTT).

The CICIoMT2024 brings a novel processing pipeline that enables data processing
for multiple protocols.

The main contributions of this research are:
+ **Development of a Comprehensive IoMT Security Dataset:** includes 18
different cyberattacks against a diverse set of 40 IoMT devs, Also this contains
research protocols namely Wi-Fi, MQTT, and Bluetooth protocols.
+ **Innovative methodology in iomt attack simulation and data collection:** A
novel systematic approach to simulating and capturing iomt network traffic under
various cyberattack scenarios. Considering the complex network of healthcare
including DDoS, DoS, Recon, MQTT, and spoofing, using a combination of real and
simulated devices. They provide advance network monitoring techniques and
specialized hardware, such as network taps, ensure the high fidelity of data
collection (Fidelity in the context of data science refers to the accuracy and
precision of data representations and analyses. It is a critical concept that
determines how closely a model or dataset reflects the real-world phenomena it
aims to represent
[refs](https://statisticseasily.com/glossario/what-is-fidelity-in-data-science-explained/)).
+ **Profiling iomt device lifecycle for enhanced security understanding:** This
research captures the lifecycle of these devices in different vital phases of a
device from the moment they join the network until they leave. As mobility in
healthcare organizations is considered a regular practice, profiling the
lifecycle while encompassing various operational phases like power interaction,
idle, active and interaction states becomes very important. by this research we
will learn understanding of the devices behavioral patterns by meticulously
capturing and analyzing the behavior of IoMT devices from the moment they join
the network. this research critical in identifying and mitigating potential
security vulnerabilities.
+ Multi-dimensional Evaluation: This study not only benchmarks the current state
of ML in IoMT security but also opens avenues for future exploration in
algorithm optimization and feature engineering.

**IoMT plays a critical role in medication management, wellness tracking, and
alert systems.**

IoMT enables remote care, personalized treatments, and preventive measures.

New applications are begin developed using IoMT devices in healthcare. These
solutions aim to improve the medical practice by offering comfort, remote care,
higher accuracy, and interconnection.

Many datasets compared with CICIoMT datasets such as:

+ ECU-IoHT dataset to demonstrate the exploitation of IoT devices in a
healthcare env. An analysis of attack behavior is conducted to support the
development of new security solutions comprising many real devices (MySignals,
temp sensor, BP sensor, HR sensor, Bluetooth and wireless adapter, Kali, and
Windows Laptop). Concerning the attacks launched, the authors focus on scaling,
ARP Spoofing, DoS, Smart, and injection.

```bib
@article{ahmed2021ecu,
  title={ECU-IoHT: A dataset for analyzing cyberattacks in Internet of Health Things},
  author={Ahmed, Mohiuddin and Byreddy, Surender and Nutakki, Anush and Sikos, Leslie F and Haskell-Dowland, Paul},
  journal={Ad Hoc Networks},
  volume={122},
  pages={102621},
  year={2021},
  publisher={Elsevier}
}
```

+ In another study authors introduce a dataset focused on how attacks are
  executed against IoMT topologies with a special focus on Bluetooth. 

The authors in [zubair2022secure] introduce a dataset focused on how attacks are executed
against IoMT topologies with a special focus on Bluetooth. An important
discussion on the technical aspects of this protocol is presented alongside its
applicability to the healthcare context. Multiple devices are used, and several
attacks are launched, followed by an in-depth ML analysis considering the
evaluation of multiple algorithms (e.g., Support Vector Machine, K-Means, and
Deep Neural Networks).

```bib
@article{zubair2022secure,
  title={Secure Bluetooth communication in smart healthcare systems: a novel community dataset and intrusion detection system},
  author={Zubair, Mohammed and Ghubaish, Ali and Unal, Devrim and Al-Ali, Abdulla and Reimann, Thomas and Alinier, Guillaume and Hammoudeh, Mohammad and Qadir, Junaid},
  journal={Sensors},
  volume={22},
  number={21},
  pages={8280},
  year={2022},
  publisher={MDPI}
}
```

Hussain et al. [hussain2021framework] introduce a data generation method to
support the design of IoT security solutions focused on healthcare.  This
method, named IoTFlock, enables the generation of both normal and malicious
network traffic. The dataset proposed adopted many IoMT devices and resulted
from the network traffic captured during. Several types of attacks can target
the MQTT protocol.  These attacks include Distributed Denial of Service (DDoS),
brute force, SlowITE, and MQTT publish flood attacks.

```bib
@article{hussain2021framework,
  title={A framework for malicious traffic detection in IoT healthcare environment},
  author={Hussain, Faisal and Abbas, Syed Ghazanfar and Shah, Ghalib A and Pires, Ivan Miguel and Fayyaz, Ubaid U and Shahzad, Farrukh and Garcia, Nuno M and Zdravevski, Eftim},
  journal={Sensors},
  volume={21},
  number={9},
  pages={3025},
  year={2021},
  publisher={MDPI}
}
```

NOTE: Moreover, other IoT security datasets are not necessarily focused on
healthcare applications.

در کنار موارد بالا باید بنویسیم که این مقاله حاوی چه عملیاتی هستش:

## Proposed CICIoMT2024

چه کار‌هایی در این مقاله انجام شده؟

قسمت بسیار مهمی هستش که بخش‌های آزمایشات رو مورد بررسی قرار میده که چه
ارزیابی‌هایی روی چه بخش‌هایی انجام شده؟

اینا اومدن یه دیتاستی از تمامی حملاتی که روی دستگاه‌های iomt میشد انجام داد رو
تهیه کردن که از طریق اون بشه خوراک مناسب فرایند مدل‌های ML رو تهیه کرد و برای
تحقیقات آینده بشه از طریق این دیتابیس به سیستم‌های iomt اتک زد یا حتی اتک‌هایی
که زده میشه رو تشخیص داد. چون یسری علائم داره که از طریق اون علائم میشه وجود اتک
در سیستم رو شناسایی کرد.

The main reason for the researchers to conduct this investigation was to address
the limitations of existing datasets and networking data processing pipelines in
the context of medical security, particularly for Internet of Medical Things
(IoMT) devices. They aimed to propose a realistic benchmark dataset that would
enable the development and evaluation of security solutions for healthcare
systems. Additionally, the research sought to establish a complementary baseline
to support further investigations and advancements in cybersecurity for IoMT
operations.

دیتاست قدرتمندی که از این فرایند تحقیقاتی بدست آمده:

http://205.174.165.80/IOTDataset/CIC_IOT_Dataset2023/Dataset/

### As their goal

1. Aiding researchers in creating secure Healthcare systems using ML.
2. Beyond simulating attacks, we capture the lifecycle of IoMT devices from
network entry to exit through profiling, allowing classifiers to identify device
anomalies.
3. Their results as CICIoMT2024 release into CI dataset page, demonstrates that
various methods can classify IoMT cyberattacks.

### Protocols

+ Wi-Fi
+ MQTT
+ Bluetooth

از این بخش به بعد تمام آزمایشات انجام شده، توپولژی مورد استفاده، تولید ترافیک
مخرب، و جنبه‌های پروفایلینگ دستگاه‌های iomt

جزء دسته‌بندی Predictive model ها برای کشف حملات در داخل شبکه این سیستم‌های
حیاتی استفاده می‌شود.

## CIC IoT Lab

در ابتدا محققان به دنبال یک آزمایشگاه IoT بودن که بتونن آزمایش‌های لازم رو انجام
بدن. داشتن آزمایشگاهی با نیاز‌های اونا یه مقدار دشوار بود. این دستگاه‌ها نیازمند
دستگاه‌های شبکه مثل روتر‌ها، اکسس پوینت‌ها و سویچ‌ها برای اتصال به شبکه و تیمی
باید می‌بود که قادر به راه‌اندازی تمام کانفیگ‌های جمورد نظر بود. بعد از اون خرید
این دستگاه‌ها به دلیل مقیاس بزرگ بودن و هزینه‌های متغیر نیازمند برنامه‌ریزی و
سرمایه‌گذاری مالی بود که به راحتی در دسترس نبود براشون.

موسسه کانادایی امنیت سایبری یا CIC اومد یک آزمایشگاه IoT برای اهداف این محققان
ایجاد کرد که شامل ده‌ها دستگاه اینترنت اشیا برای اهداف متنوع مانند دستگاه‌های
مراقبت از سلامت، دستگاه‌های خانه هوشمند و دستگاه‌های نسل بعدی را به همراه
سیستم‌های شبکه مانند روتر‌ها سویچ‌ها، اکسس پوینت‌ها، سرور‌ها و غیره رو به همراه
کیت‌های مانند Arduino و RPi رو کامل در اختیارشون گذاشت. یه تیم فنی متعهد به
نگهداری و مدیریت دستگاه‌های Iot فعلی و تمام تجهیزات شبکه را بهشون داد که بتونن
به سرعت نیازمندی که دارن رو رفع کنن و وارد فاز عملیاتی تحقیقشون بشن.

تو اون شکلی که توی دایرکتوری images هست میشه تجهیزاتی که بهشون دادن رو به تصویر
کشید.

## IoMT Topology

توپولوژی‌ای که برای انجام آزمایشات خود راه‌اندازی کردن شامل المان‌ها زیر بوده:

یک آیپد به عنوان remote controller

۴ تا RPi که تمام حملات از طریق اونا انجام میشه.

دستگاه‌های IoMT به از طریق یک اکسس پوینت متصل به شبکه هستند که اجازه میده این
دستگاه‌ها به اینترنت دسترسی داشته باشن از اون سمت هم اکسس پوینته به یه سویئچ
Netgear متصل هستش.

توی این توپولوژی تمام نود‌ها رو با پروتوکل مناسب شبیه‌سازی کردن:

+ ۱۵ تا نودی که با پروتوکل mqtt کار میکنن
+ ۷ تا دستگاهی که با WiFi کار می‌کنن
+ و ۱۴ دستگاهی که با بلوتوث از نوع کم مصرف کار می‌کنن

## Generation of malicious traffic

تولید ترافیک مخرب شامل اجرای حملات مختلف روی دستگاه‌های iomt هستش که برای تولید
بنچ مارک دیتاست نسبت به سناریو‌های پروژه‌های واقعی در دنیای دیجیتال هستش.

محققان چندین نوع از حملات رو انجام دادن:

+ DoS
+ DDoS
+ ARP spoofing
+ Flooding campaigns (ICMP, SYN, TCP, and UDP floods) در دستگاه‌هایی که با WiFi
کار می‌کردند.

هدف این فرایند ثبت ویژگی‌های ترافیک بدخیم و خراب‌کننده جهت تسهیل توسعه
راه‌حل‌های امنیت سایبری برای محیط‌های IoMT بود.

تمام شبیه‌سازی‌ها در برنامه IoTFlock انجام شده. در حقیقت یه تولید کننده ترافیکه

### WiFi

برای ایجاد ترافیک در پروتکل ارتباطی wifi محققان حملات ARP Spoofing برای Man in
the Middle اتک و بسیاری از حملات ICMP, CYN, TCP, و UDP رو انجام دادن که همه در
دسته‌بندی DoS و DDoS قرار دارند.

### MQTT

در طی این حملات.

در این پروتکل ارتباطی سه تا حمله انجام شد:

+ MQTT Connect Flood: در این حمله درخواست اتصال به بروکر با شدت زیاد ارسال می‌شود.
+ MQTT Publish Flood: ارسال بسته‌های مختلف به تاپیک‌های مختلف و رندوم mqtt
+ MQTT Malformed Data attack: شامل ارسال داده‌های نادرست به بروکر برای تجزیه و
  تحلیل رفتار و جمع‌آوری اطلاعات تاپیک‌های می‌شود.

در حمله آخر از ابزار MQTTSA استفاده شد و سعی در sniff و شنود بروکر با ارسال
بسته‌های مشخص داشتند تا رفتار دستگاه‌ها را بررسی کنند. در این فرایند حمله،
حمله‌کننده نام تمام تاپیک‌های mQTT که به صورت نهایی منتشر شده‌اند رو بدست میاره
و سعی میکنه که به هر تاپیک داده نادرستی رو ارسال بکنه.

هدف اصلی از این حملات بررسی و ارزیابی آسیب‌پذیری دستگاه‌های IoMT در پروتکل MQTT
می‌باشد.

شبیه‌ساز از طریق VMware image که یه سیستم عامل لینوکس ubuntu نسخه ۱۸.۰۴.۶ LTS
بوده. و شبیه ساز IoTFlock از نوع GUI رو که با C++ نوشته شده بوده مورد استفاده
قرار دادن.

### Bluetooth attacks

چگونگی انجام اتک‌ها در سیستم‌های مبتنی بر بلوتوث کم مصرف:

به طور کلی این ارزیابی برای بررسی مقاومت و تاب‌آوری دستگاه‌ها در برابر تهدیدات
امنیتی و اختلالات محیطی انجام شده‌اند.

معمولاً حمله در بستر BLE دو شرط الزامی را به همراه دارد:

۱. اجرای حمله
۲.جمع‌آوری ترافیک شبکه به روش‌ها و تکنیک‌های خاص

فناوری BLE به دلیل طراحی خاص خود، که برای مصرف پایین انرژی بهینه شده است، مانند
پروتکل‌های بی‌سیم یا شبکه‌های معمولی رفتار نمی‌کند بنابراین اجرای حملات یا ضبط
رترافیک در این فناوری نیازمند ابزار‌ها و تکنیک‌های متفاوت است.

این منابع شروع خیلی خوبی برای فهمیدن بودن:

https://www.youtube.com/watch?v=dsZN0dqh81k

این مقاله برای انجام این حملات از یک تلفن همراه هوشمند که به دستگاه BLE متصل است
استفاده کرده. بعد با استفاده از کامپیوتر فعالیت‌های بد‌افزاری رو انجام داده.

برای جست و جوی بلوتوث از کتابخونه bleak توی پایتون استفاده می‌کنن.

بعد تونستن برنامه‌ای بنویسن که تلاش کنه به دستگاه‌های مورد نظر متصل بشه و تمام
سرویس‌ها و اسپسیفیکشنشون رو دریافت کنه. اطلاعاتی که از این قسمت بدست میاد باعث
میشه که هکر‌ها بتونه دستگاه رو از عملکرد صحیح خودش خارج کنن.

بعد از اون برنامه تلاش میکنه که بسته‌هایی رو با سایز‌های مختلف بنویسه، سایزشون
بین ۲۰ تا ۸۱۰ بیات با افزایش ۱۰ بایتی بوده. دیتایی که میفرتسن چیزی شبیه
۰۱۲۳۴۵۶۷۸۹۰۱۲۳۴۵۶ که همش این اعداد پشت سر هم تکرار میشن. هر بار که ارسال موفقیت
آمیز باشه لاگ می‌ندازه. مشخص میشه که هر بسته روی چه UUID نوشته شده با موفقیت.
آدرس UUID چیزی شبیه SSID شبکه‌های بی‌سیم وای‌فای هستش که آدرس شبکه بلوتوث رو
مشخص می‌کنه.

بعد از اون برنامه وارد یک لوپی میشه که دیتا‌ها رو روی uuidها ارسال میکنه و
می‌نویسه. این نوشتن‌های پی در پی به هدف ایجاد اورلود در دستگاه و اختلال در
عملکرد صحیح دستگاه انجام میشه. که چیزی شبیه DoS اتک باشه.

دیتا ها به دو صورت خوانده میشود. اول اینکه لاگ‌های سمت دستگاه اندروید مورد بررسی
قرار میگیرد که به دستگاه اینترنت اشیا متصل است و دومی با استفاده از سنیف شبکه
بلوتوث با استفاده از بورد ubertooth هستش که از طریق کامپیوتر متصل میشه و تمام
بلوتوث‌های داخل محدوده رو باز میکنه. هدف اصلی این دو تا لاگ بررسی کردن برای
اطمینان از اینکه یک فهم کلی و کلان از رفتار دستگاه‌ها در حالت عادی و زمان شرایط
حمله داشته باشن.

این عملیات به شکل‌های مختلف انقدر تکرار میشه برای دستگاه‌های مربوط به healthcare
تا نتیجه‌اش رو به عنوان بررسی انعطاف‌پذیری و آسیب پذیری دستگاه در بستر اتک‌های
مبتنی بر BLE انجام بشه.

تست Lookee Sleep Ring: برای بررسی انعطاف پذیری دستگاه در مقابل حملات استفاده
می‌شود تا عملکرد سیستم مورد نظر را بدون وقفه مورد تایید قرار دهند.

تست Powerlabs HR Monitor Arm Band: مشابه با تست قبلی، بازوبند باید بتواند مطابق
با استاندارد‌هایی که اشاره کرده‌اند، در طی حمله عملکرد صحیح خودشان را داشته
باشند.

تست COOSPO HW807 Armband: در این حمله عملکرد این دستگاه‌های اینترنت ایا مورد
بررسی قرار می‌گیرد. که می‌تواند شامل ارسال داده‌های جعلی، سیگنال‌های مزاحم و یا
اعمال بار اضافی روی دستگاه باشند. نتیجه حمله آن است که سیستم دچار اضطراب عملکرد
یا overwhelmed شود که به این معناست، دستگاه نتوانسته به درستی به پردازش داده‌ها
یا مدیریت منابع خود ادامه دهد. همچنین در ادامه نتیجه دستگاه به خاموش شدن turned
off منجر شده باشد، نشان‌دهنده شکست کامل در عمکرد آن تحت شرایط حمله می‌باشد.
دقیقاً در جایی که از صحبت و بدون Fault بودن نرم‌افزار خود اطمینان داریم در اینجا
می‌توان دید که سخت‌افزار چقدر می‌تواند دربرابر عامل خارجی تحمل داشته باشد.

Livlov Heart Rate sensor: این نوع از سنسور ضربان قلب برای بررسی مقاومت در برابر
اتکشون هستش که ببین بدون وقفه داره کار میکنه.

نکته مهم در این بین اینه که درسته امنیت رو از نظر نرم‌افزاری نگاه کردیم، ولی
نکته مهم اینه که اگر کاری بکنن یا حمله‌ای انجام بشه که سیستم از حالت عادی خودش
خارج بشه دیگه اون نرم‌افزاره که دیگه نمیتونه کارشو بکنه پس عملاً اختلال تو سیستم
ایجاد کردن.

دستگاه Wellue O2 Ring: این دستگاه قشنگ به عملیات خودش ادامه میشه بدون وقفه در
هنگام اتک‌ها

دستگاه Lookee O2 Ring: این دستگاه نسبت به اتک اونا آسیب‌پذیر بوده. در طی اجرا
دستگاه کاملاً دچار اضطراب و overwhelmed شده و خاموش شد.

دستگاه checkme BP2A: این دستگاه عملکرد متفاوتی رو از خودش نشون داد. موقعی که
داشته داده رو حین حمله ذخیره می‌کرده اما این داده‌ها رو فقط زمانی ارسال کرده که
اتال بلوتوث دوباره برقرار بوده. این رفتار می‌تواند نشان‌دهنده طراحی خاص دستگاه
باشد که امنیت داده‌ها را حفظ می‌کند و ارسال آن‌ها در زمان‌هایی که اتصال بلوتوث
قطع یا نامن است جلوگیری می‌کند.

دستگاه SleepU Sleep Oxygen Monitor: در برابر حملاتی که انجام شده کاملاً مقاومت داشته.

Rhythm+2.0 (Scosche): کاملاً تحت تاثیر حمله قرار گرفت به طوری که دستگاه کاملاً
در شرایط اضطراب قرار گرفت و خاموش شد.

دستگاه Wellue Pulsebit EX: این دستگاه در مقابل حملات مقاومت کرد و به عملیات خودش
بدون قطعی ادامه داد.

Checkme O2 Smart Pulse Oximeter: این دستگاه نسبت به حملاتی که انجام شد مقاومت
داشت و به عملیات استاندارد خودش ادامه داد.

دستگاه Kinsa Thermometer: کاملاً تحت تاثیر حمله قرار گرفت و رفتار متفاوتی داشت.
در هنگام حمله دستگاه قادر به ریست کردن connection با خاموش کردن دماسنج نبود.
تنها راه ریست کردن connection خالی کردن باطری بود.

NOTE:

لازم به ذکر است که تمام حملات صورت گرفته کاملاً در محیطی ایزوله از هر گونه
سیگنال خارجی بود که ممکن است با ترافیک شبکه جمع‌آوری شده تداخله داشته باشد.

## IoMT profiling

درک کامل رفتار جنبه‌های مختلف عملیاتی که دستگاه‌های IoMT انجام میدن بسیار حیاتیه
برای بهبود امنیت سیستم. ارزیابی پروفایل‌های IoMT قابلیت کلاسیفایر‌ها رو برای
تشخیص ناهنجاری‌ها در عملیات دستگاه‌های Healthcare را با مشخص کردن رفتار وخیم یا
عادی شبکه بهبود می‌بخشد. در تسک‌هاتی کلاسیفای نشده، الگو‌های دیده نشده ممکن است
فعالیت‌های مخرب و حملات zero-day را نشان دهند.

حمله zero-day به نوعی حمله سایبری اشاره دارد که یک آسیب‌پذیری نا شناخته یا
به‌تازگی کشف شده در نرم‌افزار، سخت‌افزار یا سیستم استفاده می‌کند.

به این خاطر اسم آن را zero day attack گذاشتن که توسعه‌دهنده یا مالک سیستم هیچ
زمانی برای شناسایی و رفع آسیب‌پذیری قبل از وقوع حملات نگذاشته است.

در این تحقیق تمامی حملات مورد نظر انجام شده است که توسعه‌دهندگان و شرکت‌ها با
توجه به این حملات هیچ وقت گرفتار zero-day attack نشوند.

ویژگی‌های اصلی حملات
[zero-day](https://en.wikipedia.org/wiki/Zero-day_vulnerability): 

+ آسیب‌پذیری ناشناخته: آسیهب‌پذیری که هنوز توسط تیم امنیتی یا تیم توسعه کشف یا
  رفع نشده است.
+ غافلگیری: به دلیل عهدم آگاهی از آسیب‌پذیری، سیستم‌ها در برابر این نوع حملات
  کامل آسیب‌پذیر هستند.
+ سوء‌استفاده یا Exploit: مهاجمان معمولاً از کد یا تکنیک‌هایی برای بهره‌برداری
  از آسیب‌پذیری استفاده می‌کنند.

### Power experiments

در این قسمت آزمایشات برای مصرف انرژی دستگاه‌های مجهز به Wi-Fi مورد بررسی قرار
گرفته. این آزمایش تلاش می‌کند تا رتفار دستگاه‌های wi-fi را از نظر مصرف انرژی و
ارسال داده‌ها در هنگام روشن و خاموش بودن را به دقت تحلیل کند. این آزمایش تنها
روی هفت دستگاه که Wi-Fi هستند تمرکز دارد و دستگاه‌های MQTT شبیه‌سازی نشده‌اند.
برای انجام این آزمایش:

تمام دستگاه‌ها از شبکه خارج شده‌اند و به جایی متصل نیستند.  تنها دستگاه متصل به
شبکه یک دستگاه آیپد است که برای کنترل و نظارت بر سایر دستگاه‌ها استفاده می‌شود.
حتی دستگاه‌های RPi نیز در شبکه نیستند.

مراحل زیر به صورت کلی انجام شده:

در مرحله اول دستگاه مورد نظر روشن شد و رفتار آن برای مدت ۲ دقیقه با استفاده از
فیلتر آدرس MAC ثبت شد.

در مرحله دوم، پس از این مدت دستگاه خاموش می‌شود و فرایند ثبت داده‌ها برای ۳
دقیقه دیگر ادامه پیدا می‌کند تا هر بسته اطلاعاتی باقیمانده شناسایی شود یا
اطمینان حاصل شود که دیگر هیچ بسته‌ای از دستگاه ارسال نمی‌شود.

فرایند انجام شده دقیقاً همانند فرایندی است که در بدست آوردن دیتاست CICIoT2021
انجام شده بود. نکته قابل توجه آن است که برخی از دستگاه‌ها کلید روشن/خاموش
نداشتند و برای انجام آزمایشات نیاز به انجام تنظیماتی داشتند:

+ Singcall Sensor
+ SOS Multifunctional Page
+ Sense U Baby

### Idle experiments

آزمایشاتی است که تنها در زمان روشن بودن دستگاه ولی در حالی که هیچ داده‌ای منتقل
نمی‌کردن، انجام می‌شود. انجام این آزمایش به محققان اجازه داد که رفتار حالت عادی
و baseline شبکه رو بهتر متوجه بشن. در این آزمایش ۱۳ ساعت عملیات بررسی و آزمایش
طول کشید. آزمایشات بین دو شب از ساعت ۶ عصر تا تا ۷ صبح برای اطمینان از اینکه هیچ
تعاملی دستگاه‌ها ندارند انجام شد.

### Active experiments

شامل دستگاه‌هایی می‌شود که وظایف موردنظر خود را انجام می‌دادند و ترافیک عادی را
در شبکه بابت عملیات خود ایجاد می‌کردند.

### Interaction experiments

این قسمت از آزمایشات روی تعامل با دستگاه‌ها متمرکز است که به صورت انجام شده:

+ فیزیکی: کاربر مستقیماً با دستگاه ارتباط برقرار می‌کند.
+ دیجیتالی: برنامه‌ها با یکدیگر ارتباط می‌گیرند و ارسال داده را انجام می‌دهند.

سه نوع تعامل بررسی شده است:

تعامل فیزیکی:

+ این آزمایش‌ها زمانی انجام شده که دستگاهن دارای دکمه‌های فیزیکی بوده
+ آزمایش‌ها با ترکیب تعامل فیزیکی و شبکه‌های محلی یا شبکه‌های گسترده صورت گرفته:
  + در شبکه لوکال: اپلیکیشن و دستگاه در یک شبکه قرار داشتند.
  + در شبکه WAN: اپلیکیشن از شبکه‌ای متفاوت نسبت به دستگاه متصل بوده.

تعامل در شبکه محلی:

در این آزمایش‌ها از اپلیکشن‌های همراه دستگاه استفاه شده است. اپلیکیشن و دستگاه
هر دو در یک شبکه با استفاده از WiFi بوده‌اند. برای مثال روشن و خاموش کردن دستگاه
از طریق اپلیکیشن در خانه.

در تعامل با شبکه گسترده هم همینطور بوده، اپلیکیشن همراه دستگاه به شبکه‌ای متفاوت
متصل بوده و کنترل دستگاه از راه دور مثلا روشن کردن دستگاه خانه از دفتر کار صورت
گرفته بود.

## Machine Learning Evaluation

آزمایشاتی که انجام شده آنقدر باعث تولید دیتا شده که میشه ارزیابی‌هایی رو برای
تشخیص حمله در سیستم‌های IoMT مورد استفاده قرار داد. از جمله این مدل‌های یادگیری
ماشینی هستند که می‌توانند در این بین مورد استفاده قرار بگیرند:

+ Logistic Regression
+ Random Forest
+ Adaboost
+ Deep Neural Network (DNN)

کلاسیفای کردنشون به صورت وخیم بودن و حمله، دسته‌بندی نوع حمله، حمله وخیم،
اسپوفینگ، recon، MQTT، DoS و DDoS.