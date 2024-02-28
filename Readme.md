# TOCFL Learner Corpus

## Introduction
We constructed a TOCFL learner corpus for Chinese grammatical error diagnosis. We collected essays from the Test Of Chinese as a Foreign Language (TOCFL) and annotated grammatical errors using hierarchical tagging sets. Two kinds of error classifications were used simultaneously to tag grammatical errors. The first capital letter of each error tags denotes the coarse-grained surface differences, while the subsequent lowercase letters denote the fine-grained linguistic categories. A total of 33,835 grammatical errors in 2,837 essays and their corresponding corrections were manually annotated. We then used the Standard Generalized Markup Language to format learner texts and annotations along with learners’ accompanying metadata. The following figure shows an example. This essay was given an identification number “0612”, and was written in “2009年5月” (‘May 2009’) by a “B1”-level learner with “韓語” (‘Korean’) as his/her L1. The topic of this “記敘文” (‘narrative-style’) essay is “最 難忘的購物經驗” (‘My memorable shopping experience’), and was given a score of “4”. A number of errors were annotated. For example, the first error occurred in the first paragraph starting and ending at position 105, meaning that a word “是” (‘is’) is missing between “有時候” (‘sometimes’) and “比” (‘than’). It was annotated using an error tag “Mshi”, in which the first capital letter denotes the coarse-grained surface difference, while the subsequent lowercase letters denote the fine-grained linguistic category. In the fourth paragraph, “那時候” (‘that time’) was put in a wrong position resulting in a “Wtime” error tag denoting a time phrase in the wrong order and the word “了” (‘le’) was annotated as “Rasp” denoting a redundant aspectual particle that should be removed. The annotation can yield the correct sentence “記得那時候讀書讀得不太好” (‘Recalling that I didn’t study well at that time’).

```
<ESSAY id="0612" style="記敘文" title="最難忘的購物經驗" score="4" date="2009年5月">
                <LEARNER>
                    <L1>韓語</L1>
                    <CEFL>B1</CEFL>
                </LEARNER>
                <TEXT>
                    <P>
                        …… 在星巴克讀書，雖然需要付錢，可是我覺得有時候比圖書館好多的地方。
                    </P>
                    <P>
                        我喝咖啡的時候，常喝美式咖啡。……
                    </P>
                    <P>
                        有一天，我去星巴克，……
                    </P>
                    <P>
                        …… 那時候記得讀書讀得不太好了。以後也不常去那裏的星巴克了。
                    </P>
                </TEXT>
                <MISTAKE paragraph="1" start_off="105" end_off="105">
                    <TYPE>Mshi</TYPE>
                    <CORRECTION>是</CORRECTION>
                </MISTAKE>
                ……
                <MISTAKE paragraph="4" start_off="33" end_off="37">
                    <TYPE>Wtime</TYPE>
                    <CORRECTION>記得那時候</CORRECTION>
                </MISTAKE>
                <MISTAKE paragraph="4" start_off="45" end_off="45">
                    <TYPE>Rasp</TYPE>
                    <CORRECTION>null</CORRECTION>
                </MISTAKE>
                ….
            </ESSAY>
```

## Statistics
|  CEFR | #Title | #Essay | #Char     | Ratio% |
|:-----:|--------|--------|-----------|--------|
| A2    | 21     | 850    | 131,684   | 29.96% |
| B1    | 24     | 1,388  | 540,286   | 48.93% |
| B2    | 14     | 503    | 280,239   | 17.73% |
| C1    | 3      | 96     | 50,079    | 3.38%  |
| Total | 62     | 2,837  | 1,002,288 | 100%   |


## Citations
Lung-Hao Lee, Yuen-Hsien Tseng, and Li-Ping Chang (2018). [Building a TOCFL Learner Corpus for Chinese Grammatical Error Diagnosis.](https://aclanthology.org/L18-1363.pdf) In *Proceedings of LREC'18*, pp. 2298-2304.

