# प्रोग्रामिंग भाषाओं और व्यापार के उपकरण का परिचय

यह पाठ प्रोग्रामिंग भाषाओं की मूल बातें शामिल करता है। यहां शामिल विषय आज की अधिकांश आधुनिक प्रोग्रामिंग भाषाओं पर लागू होते हैं। 'टूल ऑफ़ ट्रेड' सेक्शन में, आप उपयोगी सॉफ़्टवेयर के बारे में जानेंगे जो आपको डेवलपर के रूप में मदद करता है।

![इंट्रो प्रोग्रामिंग](/sketchnotes//webdev101-programming.png)
>[टोमोमी इमुरा](https://twitter.com/girlie_mac) द्वारा स्केचनेट

## पूर्व व्याख्यान प्रश्नोत्तरी
[पूर्व व्याख्यान प्रश्नोत्तरी](https://ashy-river-0debb7803.1.azurestaticapps.net/quiz/1?loc=hi)

## परिचय

इस पाठ में, हम कवर करेंगे:

- प्रोग्रामिंग क्या है?
- प्रोग्रामिंग भाषाओं के प्रकार
- एक प्रोग्राम के बुनियादी तत्व
- पेशेवर डेवलपर के लिए उपयोगी सॉफ्टवेयर और टूलिंग

## प्रोग्रामिंग क्या है?

प्रोग्रामिंग (कोडिंग के रूप में भी जाना जाता है) एक डिवाइस, जैसे कि कंप्यूटर या मोबाइल डिवाइस, को निर्देश लिखने की प्रक्रिया है। हम इन निर्देशों को एक प्रोग्रामिंग भाषा के साथ लिखते हैं, जो तब डिवाइस द्वारा व्याख्या की जाती है। निर्देशों के इन सेटों को विभिन्न नामों से संदर्भित किया जा सकता है, लेकिन *प्रोग्राम*, *कंप्यूटर प्रोग्राम*, *एप्लिकेशन(ऐप)*, और *निष्पादन योग्य* कुछ लोकप्रिय नाम हैं.

एक *प्रोग्राम* कुछ भी हो सकता है जो कोड के साथ लिखा गया है; वेबसाइट, गेम और फ़ोन ऐप प्रोग्राम हैं। हालांकि, कोड लिखे बिना प्रोग्राम बनाना संभव है, अंतर्निहित तर्क की व्याख्या डिवाइस से की जाती है और उस तर्क को कोड के साथ लिखे जाने की सबसे अधिक संभावना है। एक प्रोग्राम जो *रनिंग* या *एक्जीक्यूटिंग कोड* निर्देश कर रहा है। जिस उपकरण के साथ आप वर्तमान में इस पाठ को पढ़ रहे हैं, वह आपकी स्क्रीन पर प्रिंट करने के लिए एक प्रोग्राम चला रहा है।

✅ थोड़ा अनुसंधान करें: कौन  दुनिया का पहला कंप्यूटर प्रोग्रामर माना जाता है ?

## प्रोग्रामिंग भाषाएँ

प्रोग्रामिंग भाषाओं का एक मुख्य उद्देश्य है: डेवलपर्स को डिवाइस पर भेजने के लिए निर्देशों का निर्माण करना। डिवाइस केवल बाइनरी (1s और 0s) को समझ सकते हैं, और *सबसे अधिक* डेवलपर्स के लिए जो संवाद करने का एक बहुत ही कुशल तरीका नहीं है। प्रोग्रामिंग भाषाएं मनुष्य और कंप्यूटर के बीच संचार के लिए एक वाहन हैं।

प्रोग्रामिंग भाषाएँ विभिन्न स्वरूपों में आती हैं और विभिन्न उद्देश्यों की पूर्ति कर सकती हैं। उदाहरण के लिए, जावास्क्रिप्ट का उपयोग मुख्य रूप से वेब अनुप्रयोगों के लिए किया जाता है, जबकि बैश मुख्य रूप से ऑपरेटिंग सिस्टम के लिए उपयोग किया जाता है।

*निम्न स्तर की भाषाएं* आमतौर पर निर्देशों की व्याख्या करने के लिए एक उपकरण के लिए * उच्च स्तरीय भाषाओं की तुलना में कम चरणों की आवश्यकता होती है। हालांकि, उच्च स्तरीय भाषाओं को लोकप्रिय बनाने वाली इसकी पठनीयता और समर्थन है। जावास्क्रिप्ट को एक उच्च स्तरीय भाषा माना जाता है.

निम्न कोड जावास्क्रिप्ट के साथ एक उच्च स्तर की भाषा और एआरएम विधानसभा कोड के साथ निम्न स्तर की भाषा के बीच अंतर को दर्शाता है।

```javascript
let number = 10
let n1 = 0, n2 = 1, nextTerm;

for (let i = 1; i <= number; i++) {
    console.log(n1);
    nextTerm = n1 + n2;
    n1 = n2;
    n2 = nextTerm;
}
```

```c
 area ascen,code,readonly
 entry
 code32
 adr r0,thumb+1
 bx r0
 code16
thumb
 mov r0,#00
 sub r0,r0,#01
 mov r1,#01
 mov r4,#10
 ldr r2,=0x40000000
back add r0,r1
 str r0,[r2]
 add r2,#04
 mov r3,r0
 mov r0,r1
 mov r1,r3
 sub r4,#01
 cmp r4,#00
 bne back
 end
```

मानो या न मानो, *वे दोनों एक ही काम कर रहे हैं*: 10 तक एक फाइबोनैचि अनुक्रम मुद्रित करना।

✅ एक फाइबोनैचि अनुक्रम को संख्याओं के एक सेट के रूप में [परिभाषित](https://en.wikipedia.org/wiki/Fibonacci_number) किया जाता है जैसे कि प्रत्येक संख्या दो पूर्ववर्ती का योग है, जिसकी शुरुआत 0 और 1 से होती है।

## एक प्रोग्राम के तत्व

किसी प्रोग्राम में एक निर्देश को एक *स्टेटमेंट* कहा जाता है और इसमें आमतौर पर एक कैरेक्टर या लाइन स्पेस होता है, जो उन सिरों को चिह्नित करता है, जहां से निर्देश समाप्त होता है, या *टर्मिनेट* होता है। कैसे एक कार्यक्रम समाप्त होता है प्रत्येक भाषा के साथ बदलता रहता है।

अधिकांश प्रोग्राम उपयोगकर्ता या कहीं और से डेटा का उपयोग करने पर निर्भर करते हैं, जहां कथन निर्देशों को पूरा करने के लिए डेटा पर भरोसा कर सकते हैं। डेटा बदल सकता है कि कोई प्रोग्राम कैसे व्यवहार करता है, इसलिए प्रोग्रामिंग भाषाएँ अस्थायी रूप से डेटा को संग्रहीत करने का एक तरीका है जो बाद में उपयोग किया जा सकता है। इस डेटा को *वैरिएबल* कहा जाता है। चर ऐसे कथन हैं जो किसी डिवाइस को उसकी मेमोरी में डेटा को बचाने का निर्देश देते हैं। कार्यक्रमों में विविधताएं बीजगणित में लोगों के समान हैं, जहां उनका एक अनूठा नाम है और समय के साथ उनका मूल्य बदल सकता है।

एक मौका है कि कुछ बयानों को डिवाइस द्वारा निष्पादित नहीं किया जाएगा। यह आमतौर पर डिज़ाइनर द्वारा लिखा जाता है जब डेवलपर द्वारा लिखा जाता है या जब कोई अप्रत्याशित त्रुटि होती है तो दुर्घटना से। किसी एप्लिकेशन का इस प्रकार का नियंत्रण उसे अधिक मजबूत और बनाए रखने योग्य बनाता है। आमतौर पर नियंत्रण में ये परिवर्तन तब होते हैं जब कुछ निर्णय मिलते हैं।  `if..else` स्टेटमेंट आधुनिक प्रोग्रामिंग भाषाओं में एक सामान्य विवरण यह नियंत्रित करने के लिए कि प्रोग्राम कैसे चलाया जाता है।

✅ आप बाद के पाठों में इस प्रकार के कथन के बारे में अधिक जानेंगे

## व्यापार के उपकरण

[![व्यापार के उपकरण](https://img.youtube.com/vi/69WJeXGBdxg/0.jpg)](https://youtube.com/watch?v=69WJeXGBdxg "व्यापार के उपकरण")

इस अनुभाग में, आप कुछ सॉफ़्टवेयर के बारे में जानेंगे जो आपको अपने व्यावसायिक विकास की यात्रा शुरू करने के दौरान बहुत उपयोगी लग सकते हैं .

एक **विकास पर्यावरण** उपकरण और सुविधाओं का एक अनूठा सेट है जो एक डेवलपर सॉफ्टवेयर लिखते समय अक्सर उपयोग करेगा। इन उपकरणों में से कुछ को एक डेवलपर विशिष्ट आवश्यकताओं के लिए अनुकूलित किया गया है, और समय के साथ बदल सकता है यदि कोई डेवलपर काम या व्यक्तिगत परियोजनाओं में प्राथमिकताएं बदलता है, या जब वे एक अलग प्रोग्रामिंग भाषा का उपयोग करते हैं। विकास का वातावरण डेवलपर्स के रूप में अद्वितीय है जो उनका उपयोग करते हैं।

### एडिटर्स 

सॉफ्टवेयर विकास के लिए सबसे महत्वपूर्ण उपकरणों में से एक एडिटर्स है। एडिटर्स वे होते हैं जहाँ आप अपना कोड लिखते हैं और कभी-कभी जहाँ आप अपना कोड चलाते हैं।

डेवलपर्स कुछ अतिरिक्त कारणों से एडिटर्स पर भरोसा करते हैं:

- *डिबगिंग* कोड के माध्यम से कदम से, लाइन के द्वारा बग और त्रुटियों की खोज करना। कुछ एडिटर्स में डिबगिंग क्षमताएं होती हैं, या उन्हें विशिष्ट प्रोग्रामिंग भाषाओं के लिए अनुकूलित और जोड़ा जा सकता है।.  
- *सिंटेक्स हाइलाइटिंग* कोड के लिए रंगों और पाठ स्वरूपण को जोड़ता है, यह पढ़ना आसान बनाता है। अधिकांश एडिटर अनुकूलित सिंटैक्स हाइलाइटिंग की अनुमति देते हैं.
- *एक्सटेंशन और एकीकरण* डेवलपर्स के लिए जो अतिरिक्त हैं, डेवलपर्स के लिए, अतिरिक्त टूल तक पहुंच के लिए जो कि आधार एडिटर में निर्मित नहीं हैं। उदाहरण के लिए, कई डेवलपर्स को अपने कोड को दस्तावेज करने और यह समझाने का तरीका भी चाहिए कि यह कैसे काम करता है और टाइपोस की जांच के लिए वर्तनी जांच एक्सटेंशन स्थापित करेगा। इनमें से अधिकांश परिवर्धन एक विशिष्ट एडिटर के भीतर उपयोग के लिए हैं, और अधिकांश एडिटर उपलब्ध एक्सटेंशन की खोज करने का एक तरीका है।
- *अनुकूलन* अधिकांश एडिटर अत्यंत अनुकूलन योग्य हैं, और प्रत्येक डेवलपर का अपना विशिष्ट विकास वातावरण होगा जो उनकी आवश्यकताओं के अनुरूप होगा। कई भी डेवलपर्स को अपना विस्तार बनाने की अनुमति देते हैं।

#### लोकप्रिय एडिटर्स और वेब डेवलपमेंटका एक्सटेंशन

- [Visual Studio Code](https://code.visualstudio.com/)
  - [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
  - [Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack)
  - [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Atom](https://atom.io/)
  - [spell-check](https://atom.io/packages/spell-check)
  - [teletype](https://atom.io/packages/teletype)
  - [atom-beautify](https://atom.io/packages/atom-beautify)

### ब्राउज़र्स

एक अन्य महत्वपूर्ण उपकरण ब्राउज़र है। वेब डेवलपर ब्राउज़र पर भरोसा करते हैं कि यह देखने के लिए कि उनका कोड वेब पर कैसे चलता है, इसका उपयोग वेब पेज के दृश्य तत्वों को देखने के लिए किया जाता है जो एडिटर में लिखे गए हैं, जैसे की HTML। 

कई ब्राउज़र *डेवलपर टूल*(DevTools) के साथ आते हैं, जिसमें डेवलपर्स को अपने एप्लिकेशन के बारे में महत्वपूर्ण अंतर्दृष्टि एकत्र करने और कैप्चर करने में मदद करने के लिए उपयोगी सुविधाओं और जानकारी का एक सेट होता है। उदाहरण के लिए: यदि किसी वेब पेज में त्रुटियां हैं, तो कभी-कभी यह जानना उपयोगी होता है कि वे कब हुए। एक ब्राउज़र में DevTools इस जानकारी को पकड़ने के लिए कॉन्फ़िगर किया जा सकता है।

#### लोकप्रिय ब्राउज़रों और DevTools

- [Edge](https://docs.microsoft.com/microsoft-edge/devtools-guide-chromium/?WT.mc_id=academic-77807-sagibbon)
- [Chrome](https://developers.google.com/web/tools/chrome-devtools/)
- [Firefox](https://developer.mozilla.org/docs/Tools)

### कमांड लाइन टूल्स

कुछ डेवलपर्स अपने दैनिक कार्यों के लिए कम ग्राफ़िकल दृश्य पसंद करते हैं और इसे प्राप्त करने के लिए कमांड लाइन पर भरोसा करते हैं। विकासशील कोड के लिए महत्वपूर्ण मात्रा में टाइपिंग की आवश्यकता होती है, और कुछ डेवलपर्स कीबोर्ड पर अपने प्रवाह को बाधित नहीं करना पसंद करते हैं और डेस्कटॉप विंडो के बीच स्वैप करने के लिए कीबोर्ड शॉर्टकट का उपयोग करेंगे, विभिन्न फ़ाइलों पर काम करेंगे, और टूल का उपयोग करेंगे। अधिकांश कार्यों को एक माउस के साथ पूरा किया जा सकता है, लेकिन कमांड लाइन का उपयोग करने का एक लाभ यह है कि माउस और कीबोर्ड के बीच स्वैपिंग की आवश्यकता के बिना कमांड लाइन टूल के साथ बहुत कुछ किया जा सकता है। कमांड लाइन का एक और लाभ यह है कि वे कॉन्फ़िगर करने योग्य हैं और आप अपने कस्टम कॉन्फ़िगरेशन को सहेज सकते हैं, इसे बाद में बदल सकते हैं और इसे नई विकास मशीनों में भी आयात कर सकते हैं। क्योंकि विकास वातावरण प्रत्येक डेवलपर के लिए बहुत अनूठा है, कुछ कमांड लाइन का उपयोग करने से बचेंगे, कुछ इस पर पूरी तरह से भरोसा करेंगे, और कुछ दोनों का मिश्रण पसंद करते हैं।

### लोकप्रिय कमांड लाइन विकल्प

आपके द्वारा उपयोग किए जाने वाले ऑपरेटिंग सिस्टम के आधार पर कमांड लाइन के विकल्प अलग-अलग होंगे.

*💻 = ऑपरेटिंग सिस्टम पर प्रीइंस्टॉल्ड आता है.*

#### विंडोज

- [Powershell](https://docs.microsoft.com/powershell/scripting/overview?view=powershell-7/?WT.mc_id=academic-77807-sagibbon) 💻
- [Command Line](https://docs.microsoft.com/windows-server/administration/windows-commands/windows-commands/?WT.mc_id=academic-77807-sagibbon) (also known as CMD) 💻
- [Windows Terminal](https://docs.microsoft.com/windows/terminal/?WT.mc_id=academic-77807-sagibbon)
- [mintty](https://mintty.github.io/)
  
#### मैक ओएस

- [Terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac) 💻
- [iTerm](https://iterm2.com/)
- [Powershell](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-macos/?view=powershell-7&WT.mc_id=academic-77807-sagibbon)

#### लिनक्स

- [Bash](https://www.gnu.org/software/bash/manual/html_node/index.html) 💻
- [KDE Konsole](https://docs.kde.org/trunk5/en/konsole/konsole/index.html)
- [Powershell](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-linux/?view=powershell-7&WT.mc_id=academic-77807-sagibbon)

#### लोकप्रिय कमांड लाइन टूल्स

- [Git](https://git-scm.com/) (💻 अधिकांश ऑपरेटिंग साइटम पर)
- [NPM](https://www.npmjs.com/)
- [Yarn](https://classic.yarnpkg.com/en/docs/cli/)

### प्रलेखन

जब कोई डेवलपर कुछ नया सीखना चाहता है, तो वे इसका उपयोग करने के तरीके जानने के लिए प्रलेखन की ओर रुख करेंगे। डेवलपर्स अक्सर टूल और भाषाओं का सही तरीके से उपयोग करने के लिए, और यह भी कि यह कैसे काम करता है के गहन ज्ञान प्राप्त करने के लिए मार्गदर्शन के लिए प्रलेखन पर भरोसा करते हैं।

#### वेब विकास पर लोकप्रिय प्रलेखन

- [Mozilla Developer Network (MDN)](https://developer.mozilla.org/docs/Web), Mozilla से, [Firefox](https://www.mozilla.org/firefox/) के प्रकाशक
- [Frontend Masters](https://frontendmasters.com/learn/)
- [Web.dev](https://web.dev), Google की ओर से, [Chrome](https://www.google.com/chrome/) के प्रकाशक
- [Microsoft के अपने डेवलपर दस्तावेज़](https://docs.microsoft.com/microsoft-edge/#microsoft-edge-for-developers), के लिए [Microsoft Edge](https://www.microsoft.com/edge)

✅ कुछ शोध करें: अब जब आप वेब डेवलपर के परिवेश की मूल बातें जानते हैं, तो इसकी तुलना वेब डिज़ाइनर के परिवेश से करें।

---

## 🚀 चुनौती

कुछ प्रोग्रामिंग भाषाओं की तुलना करें। जावास्क्रिप्ट बनाम जावा के कुछ विशिष्ट लक्षण क्या हैं? COBOL बनाम GO के बारे मे?

## व्याख्यान उपरांत प्रश्नोत्तरी
[व्याख्यान उपरांत प्रश्नोत्तरी](https://ashy-river-0debb7803.1.azurestaticapps.net/quiz/2?loc=hi)

## समीक्षा और स्व अध्ययन

प्रोग्रामर के लिए उपलब्ध विभिन्न भाषाओं पर थोड़ा अध्ययन करें। एक भाषा में एक पंक्ति लिखने का प्रयास करें, और फिर इसे दो अन्य में फिर से लिखें। आप क्या सीखते हैं?

## असाइनमेंट

[डॉक्स पढ़ना](assignment.hi.md)