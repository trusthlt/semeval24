# SemEval 2024 Task 5: The Legal Argument Reasoning Task in Civil Procedure
> ### 2024-01-29: ❗ The end of the evaluation phase is approaching. We have extended the deadline by 1 day to 2024-02-01 00:00:00 UTC. You can check the server time on the codalab competition page!
>

> ### 2024-01-09: The test partition has been sent out! If you have not received it, please contact [lena.held@tu-darmstadt.de](mailto:lena.held@tu-darmstadt.de).
>

> ### 2023-11-28: Thank you for you patience, the CodaLab competition is now [open](https://codalab.lisn.upsaclay.fr/competitions/14817)! Make sure to check the participation rules [below](#competition-rules) 🎉
>

We present a new NLP task and dataset from the domain of the U.S. civil procedure. Each instance of the dataset consists of a general introduction to the case, a particular question, and a possible solution argument, accompanied by a detailed analysis of why the argument applies in that case. Since the dataset is based on a book aimed at law students, we believe that it represents a truly complex task for benchmarking modern legal language models.

## Task
        
The task can be formulated as follows: Given an introduction to the topic, a question and an answer candidate, classify if the given answer candidate is correct (True) or incorrect (False).

<details>
        <summary><h3>Example 1</h3></summary>

<h4>Introduction</h4> My students always get confused about the relationship between removal to federal court and personal jurisdiction. Suppose that a defendant is sued in Arizona and believes that she is not subject to personal jurisdiction there. Naturally, she should object to personal jurisdiction. [...] But generally the scope of personal jurisdiction in the federal court will be the same as that of the state court, because the Federal Rules require the federal court in most cases to conform to state limits on personal jurisdiction. Fed. R. Civ. P. 4(k)(1)(A). I’ve stumped a multitude of students on this point. Consider the following two cases to clarify the point.

<h4>Question</h4> 7. A switch in time. Yasuda, from Oregon, sues Boyle, from Idaho, on a state law unfair competition claim, seeking \$250,000 in damages. He sues in state court in Oregon. Ten days later (before an answer is due in state court), Boyle files a notice of removal in federal court. Five days after removing, Boyle answers the complaint, including in her answer an objection to personal jurisdiction. Boyle’s objection to personal jurisdiction is

<h4>Answer Candidate</h4> not waived by removal, but will be denied because the federal courts have power to exercise broader personal jurisdiction than the state courts.

<h4>Label</h4> 0

</details>
<details>
  <summary><h3>Example 2</h3></summary>

<h4>Introduction</h4> My students always get confused about the relationship between removal to federal court and personal jurisdiction. Suppose that a defendant is sued in Arizona and believes that she is not subject to personal jurisdiction there. Naturally, she should object to personal jurisdiction. [...] But generally the scope of personal jurisdiction in the federal court will be the same as that of the state court, because the Federal Rules require the federal court in most cases to conform to state limits on personal jurisdiction. Fed. R. Civ. P. 4(k)(1)(A). I’ve stumped a multitude of students on this point. Consider the following two cases to clarify the point.

<h4>Question</h4> 7. A switch in time. Yasuda, from Oregon, sues Boyle, from Idaho, on a state law unfair competition claim, seeking \$250,000 in damages. He sues in state court in Oregon. Ten days later (before an answer is due in state court), Boyle files a notice of removal in federal court. Five days after removing, Boyle answers the complaint, including in her answer an objection to personal jurisdiction. Boyle’s objection to personal jurisdiction is

<h4>Answer Candidate</h4> not waived by removal. The court should dismiss if there is no personal jurisdiction over Boyle in Oregon, even though the case was properly removed.

<h4>Label</h4> 1

</details>

## Obtaining the training/dev dataset

Please refer to these [instructions](https://github.com/trusthlt/legal-argument-reasoning-task#obtaining-the-dataset).

## CodaLab

To evaluate the submissions we are using the CodaLab competition platform. Because of the licensing restrictions of the dataset, you will have to sign up for the competition and wait for our approval. 
The CodaLab competition can be found [here](https://codalab.lisn.upsaclay.fr/competitions/14817).

## Schedule
We adhere to the schedule for SemEval24, which means the following dates:

* ~~Tasks announced (with sample data available): 17 July 2023~~
* ~~Training data ready 4 September 2023~~
* Evaluation start **10 January 2024**
* Evaluation end by by **31 January 2024**
* Paper submission due 19 February 2024
* Notification to authors 18 March 2024
* Camera ready due 01 April 2024
* SemEval workshop: June 16–21, 2024 (co-located with NAACL 2024 in Mexico City, Mexico)

## Competition Rules
- you need to be registered and approved to enter a submission in the CodaLab competition
- you can form teams and work on the task together
- external/additional data is **allowed**, however your model should be able to handle only introduction, question and answer candidate as input
- be fair and do not cheat, buying the book and copying the answers is not a valid solution ❌
- to test your submissions, you can upload a solution for the dev set in Phase 1, the maximum number of submissions is 999
- during Phase 2 (Evaluation), you have a maximum of ***5*** submissions and the ***last submission will be counted in the competition***
- an example for creating a submission can be found [here](https://codalab.lisn.upsaclay.fr/competitions/14817#participate-get_starting_kit)
- evaluation metrics and submission format information is also explained [here](https://codalab.lisn.upsaclay.fr/competitions/14817#learn_the_details-evaluation)

## Mailing list

Subscribe to our [mailing list](https://lists.ukp.informatik.tu-darmstadt.de/wws/subscribe/semeval24-legal-reasoning).

## Leaderboard
### CodaLab Leaderboard (last submission)
<table>
    <thead>
        <tr>
            <th>#</th>
            <th>User</th>
            <th>Entries</th>
            <th>Date of Last Entry</th>
            <th>Team Name</th>
            <th>f1-score</th>
            <th>accuracy</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1</td>
            <td>zhaoxf4</td>
            <td>3</td>
            <td>31.1.2024</td>
            <td>HW-TSC</td>
            <td>0.8231</td>
            <td>0.8673</td>
        </tr>
        <tr>
            <td>2</td>
            <td>irene.benedetto</td>
            <td>7</td>
            <td>26.1.2024</td>
            <td>MAINDZ</td>
            <td>0.7747</td>
            <td>0.8265</td>
        </tr>
        <tr>
            <td>3</td>
            <td>kbkrumov</td>
            <td>7</td>
            <td>31.1.2024</td>
            <td>SU-FMI</td>
            <td>0.7728</td>
            <td>0.8367</td>
        </tr>
        <tr>
            <td>4</td>
            <td>qiaoxiaosong</td>
            <td>9</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.7644</td>
            <td>0.8163</td>
        </tr>
        <tr>
            <td>5</td>
            <td>arios0</td>
            <td>4</td>
            <td>30.1.2024</td>
            <td>UTSA-NLP</td>
            <td>0.7315</td>
            <td>0.7959</td>
        </tr>
        <tr>
            <td>6</td>
            <td>kubapok</td>
            <td>10</td>
            <td>13.1.2024</td>
            <td></td>
            <td>0.6971</td>
            <td>0.7857</td>
        </tr>
        <tr>
            <td>7</td>
            <td>samyak</td>
            <td>4</td>
            <td>31.1.2024</td>
            <td>LegalSense</td>
            <td>0.6599</td>
            <td>0.7449</td>
        </tr>
        <tr>
            <td>8</td>
            <td>hrandria</td>
            <td>7</td>
            <td>29.1.2024</td>
            <td></td>
            <td>0.6327</td>
            <td>0.6939</td>
        </tr>
        <tr>
            <td>9</td>
            <td>Yuan_Lu</td>
            <td>8</td>
            <td>31.1.2024</td>
            <td></td>
            <td>0.6000</td>
            <td>0.6327</td>
        </tr>
        <tr>
            <td>10</td>
            <td>PengShi</td>
            <td>14</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.5910</td>
            <td>0.6735</td>
        </tr>
        <tr>
            <td>11</td>
            <td>msiino</td>
            <td>1</td>
            <td>31.1.2024</td>
            <td>Mistral</td>
            <td>0.5597</td>
            <td>0.5714</td>
        </tr>
        <tr>
            <td>12</td>
            <td>Hwan_Chang</td>
            <td>4</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.5556</td>
            <td>0.5918</td>
        </tr>
        <tr>
            <td>13</td>
            <td>kriti7</td>
            <td>15</td>
            <td>31.1.2024</td>
            <td></td>
            <td>0.5511</td>
            <td>0.6020</td>
        </tr>
        <tr>
            <td>14</td>
            <td>woody</td>
            <td>22</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.5510</td>
            <td>0.6633</td>
        </tr>
        <tr>
            <td>15</td>
            <td>odysseas_aueb</td>
            <td>11</td>
            <td>1.2.2024</td>
            <td></td>
            <td>0.5143</td>
            <td>0.6122</td>
        </tr>
        <tr>
            <td>16</td>
            <td>Manvith_Prabhu</td>
            <td>11</td>
            <td>31.1.2024</td>
            <td>SCaLAR Group, NITK Surathkal</td>
            <td>0.4966</td>
            <td>0.6224</td>
        </tr>
        <tr>
            <td>17</td>
            <td>lhoorie</td>
            <td>1</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.4957</td>
            <td>0.5000</td>
        </tr>
        <tr>
            <td>18</td>
            <td>yms</td>
            <td>8</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.4827</td>
            <td>0.7245</td>
        </tr>
        <tr>
            <td>19</td>
            <td>U_201060</td>
            <td>1</td>
            <td>29.1.2024</td>
            <td></td>
            <td>0.4503</td>
            <td>0.6633</td>
        </tr>
        <tr>
            <td>20</td>
            <td>langml</td>
            <td>2</td>
            <td>30.1.2024</td>
            <td>langml</td>
            <td>0.4375</td>
            <td>0.4490</td>
        </tr>
        <tr>
            <td>21</td>
            <td>lena.held</td>
            <td>2</td>
            <td>7.8.2023</td>
            <td></td>
            <td>0.4269</td>
            <td>0.7449</td>
        </tr>
    </tbody>
</table>

### Custom Leaderboard (best submission)

<table>
    <thead>
        <tr>
            <th>#</th>
            <th>User</th>
            <th>Entries</th>
            <th>Date of Entry</th>
            <th>Team Name</th>
            <th>f1-score</th>
            <th>accuracy</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1</td>
            <td>zhaoxf4</td>
            <td>3</td>
            <td>31.1.2024</td>
            <td>HW-TSC</td>
            <td>0.8231</td>
            <td>0.8673</td>
        </tr>
        <tr>
            <td>2</td>
            <td>irene.benedetto</td>
            <td>7</td>
            <td>26.1.2024</td>
            <td>MAINDZ</td>
            <td>0.7747</td>
            <td>0.8265</td>
        </tr>
        <tr>
            <td>3</td>
            <td>kbkrumov</td>
            <td>7</td>
            <td>31.1.2024</td>
            <td>SU-FMI</td>
            <td>0.7728</td>
            <td>0.8367</td>
        </tr>
        <tr>
            <td>4</td>
            <td>qiaoxiaosong</td>
            <td>9</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.7644</td>
            <td>0.8163</td>
        </tr>
        <tr>
            <td>5</td>
            <td>arios0</td>
            <td>3</td>
            <td>12.1.2024</td>
            <td>UTSA-NLP</td>
            <td>0.7341</td>
            <td>0.8061</td>
        </tr>
        <tr>
            <td>6</td>
            <td>kubapok</td>
            <td>10</td>
            <td>13.1.2024</td>
            <td></td>
            <td>0.6971</td>
            <td>0.7857</td>
        </tr>
        <tr>
            <td>7</td>
            <td>samyak</td>
            <td>4</td>
            <td>31.1.2024</td>
            <td>LegalSense</td>
            <td>0.6599</td>
            <td>0.7449</td>
        </tr>
        <tr>
            <td>8</td>
            <td>hrandria</td>
            <td>7</td>
            <td>29.1.2024</td>
            <td></td>
            <td>0.6327</td>
            <td>0.6939</td>
        </tr>
        <tr>
            <td>9</td>
            <td>PengShi</td>
            <td>13</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.6166</td>
            <td>0.6837</td>
        </tr>
        <tr>
            <td>10</td>
            <td>Yuan_Lu</td>
            <td>8</td>
            <td>31.1.2024</td>
            <td></td>
            <td>0.6000</td>
            <td>0.6327</td>
        </tr>
        <tr>
            <td>11</td>
            <td>Hwan_Chang</td>
            <td>3</td>
            <td>29.1.2024</td>
            <td></td>
            <td>0.6000</td>
            <td>0.6735</td>
        </tr>
        <tr>
            <td>12</td>
            <td>msiino</td>
            <td>1</td>
            <td>31.1.2024</td>
            <td>Mistral</td>
            <td>0.5597</td>
            <td>0.5714</td>
        </tr>
        <tr>
            <td>13</td>
            <td>kriti7</td>
            <td>15</td>
            <td>31.1.2024</td>
            <td></td>
            <td>0.5511</td>
            <td>0.6020</td>
        </tr>
        <tr>
            <td>14</td>
            <td>woody</td>
            <td>22</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.5510</td>
            <td>0.6633</td>
        </tr>
        <tr>
            <td>15</td>
            <td>Manvith_Prabhu</td>
            <td>3</td>
            <td>25.1.2024</td>
            <td>SCaLAR Group, NITK Surathkal</td>
            <td>0.5238</td>
            <td>0.6429</td>
        </tr>
        <tr>
            <td>16</td>
            <td>odysseas_aueb</td>
            <td>11</td>
            <td>1.2.2024</td>
            <td></td>
            <td>0.5143</td>
            <td>0.6122</td>
        </tr>
        <tr>
            <td>17</td>
            <td>lhoorie</td>
            <td>1</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.4957</td>
            <td>0.5000</td>
        </tr>
        <tr>
            <td>18</td>
            <td>yms</td>
            <td>8</td>
            <td>30.1.2024</td>
            <td></td>
            <td>0.4827</td>
            <td>0.7245</td>
        </tr>
        <tr>
            <td>19</td>
            <td>U_201060</td>
            <td>1</td>
            <td>29.1.2024</td>
            <td></td>
            <td>0.4503</td>
            <td>0.6633</td>
        </tr>
        <tr>
            <td>20</td>
            <td>langml</td>
            <td>2</td>
            <td>30.1.2024</td>
            <td>langml</td>
            <td>0.4375</td>
            <td>0.4490</td>
        </tr>
        <tr>
            <td>21</td>
            <td>lena.held</td>
            <td>2</td>
            <td>7.8.2023</td>
            <td></td>
            <td>0.4269</td>
            <td>0.7449</td>
        </tr>
    </tbody>
</table>
