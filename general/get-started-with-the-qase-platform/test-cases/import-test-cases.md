---
description: >-
  Learn how to import test cases into Qase in three easy steps and streamline
  your test case migration process.
---

# Import test cases

{% embed url="https://www.youtube.com/watch?v=j8hZiTea3b4" %}

### How to import test cases?

You can import your test cases into Qase in 3 easy steps.

1. **Click the "..." menu icon** in the top right-hand corner of your repository, and choose "**Import Data**" from the menu.

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595244819/d859f668c89fe20f335dc4ed/loNtdZKbSQeE0ndtXVDrWf_Mg1tPv8rznQJhMIdMh7c5gg9sE0JkcaB6a61gBWcDE5A4KvlkYGWWwbj_iDAo4lNJG4cnlAwYkcqhPso7bQyr6jf4z3JG-QMhPdsKihpjZVeQNgsvmTv9WwaY5FcToE2GDD_6qBABs7Ukn8OmiZM0CMgrwds-N1vJaw" alt=""><figcaption></figcaption></figure>

After clicking "Import Data," a pop-up will appear.

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595244899/c5bc5f60b5c3354762080a09/l1jggqTM7nZy7_WOxipsI-sJ_e4keNGwlcYLHW1xI1txg0iJqa_0402qyOSCElecwKUrX-u6Al4k0uGlOk_tC1UgLIXTQb1CXEAvFhkMIb1tfk3eZ-UCV_sSieZLN3xxnKXTGLx2mMbF8fVDpv8ifwjXMAu3a0YXgh-IWJL1YxG_u9vAXugNlUUSig" alt=""><figcaption></figcaption></figure>

2. **Select the Source type** - the TMS platform you are migrating from.

&#x20;<mark style="background-color:yellow;">If you're using MS Excel for your test cases, choose the Qase.io format when uploading your file. Ensure that</mark> [<mark style="background-color:yellow;">the headers</mark>](https://drive.google.com/file/d/1LZL0Zg2GRMOyn8TsXv-hGsuO4m6pXuxI/view?usp=drive\_link) <mark style="background-color:yellow;">in your file follow the specified format. You can download this</mark> [<mark style="background-color:yellow;">example CSV</mark> ](https://drive.google.com/file/d/1ZWEBZHNtkJZWnvNcMoNoR-mOznp-8Ahd/view)<mark style="background-color:yellow;">for reference.</mark>&#x20;

3. **Select a Suite** to act as the parent for all imported test cases. If no suite is defined, all test cases and suites will go to the project's root.

<figure><img src="../../../.gitbook/assets/Screenshot 2023-12-04 at 3.16.07 PM.png" alt=""><figcaption></figcaption></figure>

### Source Types

| Source                | Formats          | Description                                                                                                                                                 |
| --------------------- | ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Qase                  | XML / JSON / CSV | It can be helpful when you want to move test cases from one project to another and start it from scratch.                                                   |
| Test Rail             | XML / CSV        | If you want to import test cases from TestRail, the best choice is to use XML because it has a nested structure, and you will get the most accurate result. |
| Test Link             | XML              |                                                                                                                                                             |
| Zephyr Squad/Scale    | XML              |                                                                                                                                                             |
| SquashTM              | XLS              |                                                                                                                                                             |
| CucumberStudio        | XML              |                                                                                                                                                             |
| Zephyr Standalone     | XML              |                                                                                                                                                             |
| Zephyr for Jira Cloud | XML              |                                                                                                                                                             |
| TestLodge             | CSV              |                                                                                                                                                             |
| TestCollab            | XML              |                                                                                                                                                             |
| Xray                  | XML              |                                                                                                                                                             |
| TestCaseLab           | CSV              |                                                                                                                                                             |
| TestPad               | CSV              |                                                                                                                                                             |
| AllureTestOps         | CSV              |                                                                                                                                                             |
| AllureReporter        | CSV              |                                                                                                                                                             |
| qTest                 | XLS              |                                                                                                                                                             |
| PractiTest            | CSV              |                                                                                                                                                             |

### Troubleshooting <a href="#h_117d219698" id="h_117d219698"></a>

We offer many parsers for various source types, but if you encounter import issues, reach out to our support team via [email](mailto:support@qase.io) or the in-app chat.
