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
