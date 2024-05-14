# Test suites

### What is a test suite in software testing?

A test suite acts like a folder where we store our test cases organized by sections and subsections. You can create several test suites. For example, functional and non-functional test suites or anything else that should be treated as a separate group of tests.

{% embed url="https://www.youtube.com/watch?v=G5f1Ds390_E" %}

{% embed url="https://youtu.be/Gz5gfZ4_7WM" %}

### **To create a test suite:**

1.  On the "Repository" page, click the "Create new suite" button, or click "+ Suite" next to the search bar at the top.\


    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597420266/bd386696109eff5ddc570d6b/jTxtjwLUluuGX1AQ9cuK2WOzDFu8CrrP9PM3UzS-oQkOp1RYjBcmzPHHX5LVQzS-BU0K9lO6J7QxLXGvfEtnNXfnOcABRqvVNyRF2-fafAJQEha1gpWfUPGhHu8Ejx2MNki9wRPuEjWkFoldxQMivKGTz_6Wv7rPepye-px8UK9dJxuHN5FeKxnt8g" alt=""><figcaption></figcaption></figure>
2. A popup window titled "Create Suite" will appear. Now let's fill in the fields:
   * Suite name: give your test suite a descriptive name that allows you to unequivocally define which domain or area of development it will cover. Suite name is the only mandatory field to create a suite - other fields are optional and can be filled at a later stage or left empty.
   * Parent suite: it is possible to have a multi-level hierarchy of test suites, so if a suite you are configuring will be a part of a larger scope of testing scenarios, you can put it into a higher-level parent suite.
   * Description: provide additional details and context regarding which test cases should belong to a test suite.
   * Preconditions: describe the steps that should be completed before you can proceed with test cases from the newly created suite.\
     [![](https://qase.intercom-attachments-7.com/i/o/597420271/71cba06887c58ddcf4eb06c4/YSDIpfhftkdvSOpMc15\_mvfSp8iwcrry0-Ft4mJCZPiQw8Fe\_98guvwk87CSqZbcDqZN-fu1RxIcwa2N0LfwX\_QET4va08b9xpgZ8GLPnqGZebrvvAF\_VxovIgFka0\_2Lr\_pib8XSDJAZUTn4zEwNKL9xm-oSFTxSexCMRrmTpjinWhOmaKM0f\_mEg)](https://qase.intercom-attachments-7.com/i/o/597420271/71cba06887c58ddcf4eb06c4/YSDIpfhftkdvSOpMc15\_mvfSp8iwcrry0-Ft4mJCZPiQw8Fe\_98guvwk87CSqZbcDqZN-fu1RxIcwa2N0LfwX\_QET4va08b9xpgZ8GLPnqGZebrvvAF\_VxovIgFka0\_2Lr\_pib8XSDJAZUTn4zEwNKL9xm-oSFTxSexCMRrmTpjinWhOmaKM0f\_mEg)
3. To create a test suite, click "Create".
4.  The repository will now display the newly created test suite.\


    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597420280/0d5db0fc0c502949be8d99eb/855c50KLt7wgszKz6U-aBZMCOFgYKXPkvK7Ss7O1j6zZnQ4yfzJrArUGAiwEdMTP_PqBL2EBZYwfpcVAs4HtqmjsN26g6Vv3HyRWLEh5eM0C-ZSepP_y-XSFG3sftObpnG2-uY8YOB7pFRa1bNKDNs-T-7zR_dMTl_QwSlm2vA2DCm3R524-yrMHIA" alt=""><figcaption></figcaption></figure>

Once you have created one or several test suites, your repository will reflect how they are structured and related to each other.

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595235012/dfdcbe1044e27d478bfb5714/hlWTKJli8CYEId0spMk-3kOM6WjlE_QlH-q91yH5-ghuEdXe1H_CpWY_4EkI3BzMUvLbd-2M6uJCnIyhCb18zepblH9O2iKCaSv7Ea7CNtDhUbR5UTIWc0QiEYpUhHzucyjd6_odBrdzWCm4IFqNbNtrkDHEtEFD3C3CRhD0EqRv9exzEc_SJtZ9fw" alt=""><figcaption></figcaption></figure>

### Test suites controls

While in Repository view, hovering over "Test suite" reveals several controls:

* _Collapse / Expand:_ Clicking on the name of the test suite collapses or expands it.

<figure><img src="../.gitbook/assets/collapse expand.gif" alt=""><figcaption></figcaption></figure>

* _Create Case / Create Suite:_ Clicking on the "+" icon opens a menu with options to "Create Suite" or "Create Case."\


<figure><img src="../.gitbook/assets/create case suite.gif" alt=""><figcaption></figcaption></figure>

* _Edit Suite:_ Clicking on the pencil icon allows you to edit the suite itself.

<figure><img src="../.gitbook/assets/edit suite.gif" alt=""><figcaption></figcaption></figure>

* _Clone Suite:_ Clicking on the two pages icon allows you to clone the suite. You can choose the project to which you want the suite cloned, its parent suite, clone strategy, and prefix. You also have the option to clone the suite with its children (suites and cases).

<figure><img src="../.gitbook/assets/clone suite.gif" alt=""><figcaption></figcaption></figure>

* _Delete Suite:_ Clicking on the trash can icon lets you delete the suite. Once deleted, you cannot restore the suite from the "[Trash Bin.](https://docs.qase.io/general/get-started-with-the-qase-platform/test-cases/trash-bin)"

<figure><img src="../.gitbook/assets/delete suite.gif" alt=""><figcaption></figcaption></figure>

To navigate around your Suite structure easier, there are three Suite Tree layouts available, which you can toggle between using the “Views” dropdown in the top-right corner of the Repository:

[![](https://qase.intercom-attachments-7.com/i/o/595235064/62ce8efcbdd9ca0fa49eebe6/cVXPaAsOTKZqMZxugJ2vRgc79PLTOCeysHkB1PFxi8QUhn-AtSCZpzf-8EjsBlKuQEE7hfbaGRrpxK1rYmmvj\_YNBG2GIkG42vkpBOnl2tvvn43PVXWkc2pZDXRcfwzVemNEPbBaEN7nlxmLU-gIt-zOjCXjvNSkX0Yvm9ursboIS4E-TJJVL0MYdQ)](https://qase.intercom-attachments-7.com/i/o/595235064/62ce8efcbdd9ca0fa49eebe6/cVXPaAsOTKZqMZxugJ2vRgc79PLTOCeysHkB1PFxi8QUhn-AtSCZpzf-8EjsBlKuQEE7hfbaGRrpxK1rYmmvj\_YNBG2GIkG42vkpBOnl2tvvn43PVXWkc2pZDXRcfwzVemNEPbBaEN7nlxmLU-gIt-zOjCXjvNSkX0Yvm9ursboIS4E-TJJVL0MYdQ)

* Default layout also known as the “Nested Tree View” shows all of the Suites you currently have in your project; you can open up the Suite Tree sidebar to navigate from one suite to another:

<figure><img src="../.gitbook/assets/nested tree view.gif" alt=""><figcaption></figcaption></figure>

* The alternative “Folders view” layout shows only the Test Suite and Test Cases in focus, while to navigate to a different Suite, you need to select it from the sidebar. This layout proves to be a better solution for massive structures with complicated hierarchies:

<figure><img src="../.gitbook/assets/folders view.gif" alt=""><figcaption></figcaption></figure>

* Mind Map view (Beta): This view displays all the suites and test cases within a project as a mind map. It also provides the option to create quick cases or suites by clicking on the “+” icon. You can alter the hierarchy of display by dragging the suite up or down. You can also move a test case from one suite to another. Additionally, clicking on the case will allow you to update its title.

<figure><img src="../.gitbook/assets/mind map view.gif" alt=""><figcaption></figcaption></figure>

Additionally, in both the Nested Tree view and the Folders view, you can click on the “...” menu icon to Edit, Close, Select and Unselect all, Create Suite, Create Case, and Delete.\
[![](https://qase.intercom-attachments-7.com/i/o/595235110/01261a556674548aa2f2e629/EYftJ0BAW0hwf5d-QktQqiKnIT8-B9veKSpiusN-XjmknNY7CqFCf1Vzsvtt6E6A6SqQTgZePk4ONFVdL75EoZeD\_GJ3oiunL-7xIVVVAMOCAkE9EJXj7Q4eMS8Hquj6GeVnSyGmZITZ8XDrNu5FSfRLCXIF4ZCwB7hcLP7nKWCH6LO7Jwc316bNsw)](https://qase.intercom-attachments-7.com/i/o/595235110/01261a556674548aa2f2e629/EYftJ0BAW0hwf5d-QktQqiKnIT8-B9veKSpiusN-XjmknNY7CqFCf1Vzsvtt6E6A6SqQTgZePk4ONFVdL75EoZeD\_GJ3oiunL-7xIVVVAMOCAkE9EJXj7Q4eMS8Hquj6GeVnSyGmZITZ8XDrNu5FSfRLCXIF4ZCwB7hcLP7nKWCH6LO7Jwc316bNsw)



