# SemEval 2024: The Legal Argument Reasoning Task in Civil Procedure

We present a new NLP task and dataset from the domain of the U.S. civil procedure. Each instance of the dataset consists of a general introduction to the case, a particular question, and a possible solution argument, accompanied by a detailed analysis of why the argument applies in that case. Since the dataset is based on a book aimed at law students, we believe that it represents a truly complex task for benchmarking modern legal language models.

## Task
        
The task can be formulated as follows: Given an introduction to the topic, a question and an answer candidate, classify if the given answer candidate is correct (True) or incorrect (False).

### Example 1

**Introduction** My students always get confused about the relationship between removal to federal court and personal jurisdiction. Suppose that a defendant is sued in Arizona and believes that she is not subject to personal jurisdiction there. Naturally, she should object to personal jurisdiction. [...] But generally the scope of personal jurisdiction in the federal court will be the same as that of the state court, because the Federal Rules require the federal court in most cases to conform to state limits on personal jurisdiction. Fed. R. Civ. P. 4(k)(1)(A). I’ve stumped a multitude of students on this point. Consider the following two cases to clarify the point.

**Question** 7. A switch in time. Yasuda, from Oregon, sues Boyle, from Idaho, on a state law unfair competition claim, seeking \$250,000 in damages. He sues in state court in Oregon. Ten days later (before an answer is due in state court), Boyle files a notice of removal in federal court. Five days after removing, Boyle answers the complaint, including in her answer an objection to personal jurisdiction. Boyle’s objection to personal jurisdiction is

**Answer Candidate** not waived by removal, but will be denied because the federal courts have power to exercise broader personal jurisdiction than the state courts.

**Label** 0

### Example 2

**Introduction** My students always get confused about the relationship between removal to federal court and personal jurisdiction. Suppose that a defendant is sued in Arizona and believes that she is not subject to personal jurisdiction there. Naturally, she should object to personal jurisdiction. [...] But generally the scope of personal jurisdiction in the federal court will be the same as that of the state court, because the Federal Rules require the federal court in most cases to conform to state limits on personal jurisdiction. Fed. R. Civ. P. 4(k)(1)(A). I’ve stumped a multitude of students on this point. Consider the following two cases to clarify the point.

**Question** 7. A switch in time. Yasuda, from Oregon, sues Boyle, from Idaho, on a state law unfair competition claim, seeking \$250,000 in damages. He sues in state court in Oregon. Ten days later (before an answer is due in state court), Boyle files a notice of removal in federal court. Five days after removing, Boyle answers the complaint, including in her answer an objection to personal jurisdiction. Boyle’s objection to personal jurisdiction is

**Answer Candidate** not waived by removal. The court should dismiss if there is no personal jurisdiction over Boyle in Oregon, even though the case was properly removed.

**Label** 1

## Obtaining the training/dev dataset

Please refer to these [instructions](https://github.com/trusthlt/legal-argument-reasoning-task#obtaining-the-dataset).

## CodaLab

TBD

## Mailing list

Subscribe to our [mailing list](https://lists.ukp.informatik.tu-darmstadt.de/wws/subscribe/semeval24-legal-reasoning).
