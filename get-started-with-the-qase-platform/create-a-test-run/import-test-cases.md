# Import test cases

{% embed url="https://youtu.be/hEVtX_sgzEY" %}

### How to import test cases?

1. To import test cases into the Qase [project](https://help.qase.io/en/articles/5563706-projects), you need to open your project’s repository and click on the “...” icon on the top right-hand side. You will then see a menu with the option to click on “Import data”.

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595244819/d859f668c89fe20f335dc4ed/loNtdZKbSQeE0ndtXVDrWf_Mg1tPv8rznQJhMIdMh7c5gg9sE0JkcaB6a61gBWcDE5A4KvlkYGWWwbj_iDAo4lNJG4cnlAwYkcqhPso7bQyr6jf4z3JG-QMhPdsKihpjZVeQNgsvmTv9WwaY5FcToE2GDD_6qBABs7Ukn8OmiZM0CMgrwds-N1vJaw" alt=""><figcaption></figcaption></figure>

2. Once you click on “Import data”, you will see a pop-up with the option to select the format based on the source type (current TMS platform that you currently use).

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595244899/c5bc5f60b5c3354762080a09/l1jggqTM7nZy7_WOxipsI-sJ_e4keNGwlcYLHW1xI1txg0iJqa_0402qyOSCElecwKUrX-u6Al4k0uGlOk_tC1UgLIXTQb1CXEAvFhkMIb1tfk3eZ-UCV_sSieZLN3xxnKXTGLx2mMbF8fVDpv8ifwjXMAu3a0YXgh-IWJL1YxG_u9vAXugNlUUSig" alt=""><figcaption></figcaption></figure>

3. If you’re using Excel to maintain and track your test cases, you can click on the Qase.io format, and you can upload your file. However, the headers of your file are required to be in a specified format. Here’s an [example template](https://docs.google.com/spreadsheets/d/13NeOTz\_ftxZSxZmdvwCug4PIN3swjTxDmA2GR16dkZA/edit?usp=sharing) that you can download for a CSV file.
4. Once you’ve uploaded the file, you can choose a suite that will be a parent for all imported test cases. If the suite is not defined, all test cases and suites will be uploaded to the root of the project.

[![](https://qase.intercom-attachments-7.com/i/o/595244909/77be7a6612884a05369c0822/VqFEygFlBC0j9WHskgDogkfLFu\_gg4Vdf9vjd-xdenvp3KBQd\_teg9GVZQcpc44PVCgS7WUQ53RnGhR0GK9PN1DVmPT9peOxFIxb9dASRw9cdTYohcS2BWZ0HcTbP-8j1Z4iQ8eC9hH5aiYDVSNkKtUIkhbIAK-U6JnCFDTNYdn5HGYcuXLFuhi9AA)](https://qase.intercom-attachments-7.com/i/o/595244909/77be7a6612884a05369c0822/VqFEygFlBC0j9WHskgDogkfLFu\_gg4Vdf9vjd-xdenvp3KBQd\_teg9GVZQcpc44PVCgS7WUQ53RnGhR0GK9PN1DVmPT9peOxFIxb9dASRw9cdTYohcS2BWZ0HcTbP-8j1Z4iQ8eC9hH5aiYDVSNkKtUIkhbIAK-U6JnCFDTNYdn5HGYcuXLFuhi9AA)

### Source types <a href="#h_a673c8cb65" id="h_a673c8cb65"></a>

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

We have a lot of parsers for different source types that cover a lot of corner cases but not all of them. If you have problems with import, please, contact support by [email](mailto:support@qase.io) or through the chat in the app.
