# Custom fields

### What are custom fields in Qase?

Obviously, test scenarios come with all varieties of data connected to them. It is pretty much impossible for us at Qase to predict every single data point you want to record for your [Test Cases](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run), [Test Runs](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run-1), or [Defects](https://docs.qase.io/general/get-started-with-the-qase-platform/defects). So instead of trying to cover all bases or giving a bare minimum, we provide you with Custom Fields - a tool to create your own custom data entry points.

_<mark style="background-color:purple;">⚠️Custom Fields are available in</mark>_ [_<mark style="background-color:purple;">Startup</mark>_](https://help.qase.io/en/articles/5563728-startup-plan)_<mark style="background-color:purple;">,</mark>_ [_<mark style="background-color:purple;">Business</mark>_](https://help.qase.io/en/articles/5563727-business-plan)_<mark style="background-color:purple;">, and</mark>_ [_<mark style="background-color:purple;">Enterprise</mark>_](https://help.qase.io/en/articles/6640055-enterprise-plan) _<mark style="background-color:purple;">subscriptions</mark>_

{% embed url="https://youtu.be/SnXr_WPJiMc" %}

You'll need to create these Custom Fields first to be able to fill them in. To get started, navigate to the Workspace settings' "Fields" section:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597122367/191a4014043ec3de84be3310/9dkRGRx5uAm_u_fdOe5xBUnV5PZw6gaae8zvueizzh6kMbGGMxEoUYyphjUMfmZDOjqOAunvkbdb74heGqJZq7HyBhx-1WnTGtQR9u2j7ejgTYjdodVlRadQl8IkSzBN6n1e8vTdjZAcz6XdNf4nZz6Nfppj65UV_wf8TUq2At1_MMyto2na-aa0xQ" alt=""><figcaption></figcaption></figure>

### Create custom fields

Create a new Custom Field by clicking "+ Create New Custom Field", configure your Custom Field, and define what it will be representing:

* _Title:_ give a brief descriptive name to your Custom Field (Title is the only mandatory parameter).

Create a new custom field by clicking "+ Create custom field", configure your custom field, and define what it will be representing:

* _Title:_ give a brief descriptive name to your Custom Field (Title is the only mandatory parameter).\
  \
  [![](https://qase.intercom-attachments-7.com/i/o/597122368/6b2b081bb74b2ea946ed8441/IOAd6j0zBKZO6Zkz8T5A2-iFdxacMVO3Nj12JL4Ozvx\_0Ks3H4aghfqf7v4MFAwirKIhHwu2Z3g-Hw3Fnb0aD01LVSrpgBosRRKCR3fn5wxwzRGffz7tyk6ZUWoBScqGzsji8vqzCY2nKepwJXFk5o1RpcDT35-cvLYKpL45FFfAURxG9iMXr8pceg)](https://qase.intercom-attachments-7.com/i/o/597122368/6b2b081bb74b2ea946ed8441/IOAd6j0zBKZO6Zkz8T5A2-iFdxacMVO3Nj12JL4Ozvx\_0Ks3H4aghfqf7v4MFAwirKIhHwu2Z3g-Hw3Fnb0aD01LVSrpgBosRRKCR3fn5wxwzRGffz7tyk6ZUWoBScqGzsji8vqzCY2nKepwJXFk5o1RpcDT35-cvLYKpL45FFfAURxG9iMXr8pceg)
* _Entity:_ define which Qase entities your Custom Field will apply to - Test Cases, Test Runs, or Defects. This parameter is a single-choice one, so you cannot select "Test Cases" AND "Test Runs"; if you need to track similar data for both Runs and Cases, you'll need to create two separate Custom Fields for that.\
  \
  [![](https://qase.intercom-attachments-7.com/i/o/597122370/87a14b739d5e0c5c9abee4ec/nHk3s1kwtlph8ulrxWerSRlMuM8i3Ic8a1u1ve63P1lQt5XI6BYa9SiUmEiEktK6L83m7PkQ1cBknLa7zcxTdmW5BeuMSlJ\_I6Wo77dEaz-ePz5JdkSMDn2torB6O2aDU1g6tlmaL\_k7t7pY6kbZi48i0FH1h-kCkRvPYh8fnMf0g0RjeH1M-sQY)](https://qase.intercom-attachments-7.com/i/o/597122370/87a14b739d5e0c5c9abee4ec/nHk3s1kwtlph8ulrxWerSRlMuM8i3Ic8a1u1ve63P1lQt5XI6BYa9SiUmEiEktK6L83m7PkQ1cBknLa7zcxTdmW5BeuMSlJ\_I6Wo77dEaz-ePz5JdkSMDn2torB6O2aDU1g6tlmaL\_k7t7pY6kbZi48i0FH1h-kCkRvPYh8fnMf0g0RjeH1M-sQY)
* _Type:_ select from a dropdown which data type will be used in this Custom Field. Depending on the type of data selected, the options below will be different.\
  ​_NB: once a custom field has been created, its type cannot be changed._

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597122372/3e9135b28f07a4e6a3c039bb/mmxDw7R4VosOoxz9p6xEXi_G4fv-cHmKGSteiJDzckBbCrQc5EP9d0mkSGTyWmomzx9CA6_0B6PRue5NoaNyyPJM4NIcC_Uj5emli6MJziLKotxEPwKjEKFYcCBJ-ddL4-OfCrT5IMEqyXIvUargU8DCoPPt8KWgmRx5uasTNf63r7xVegvkz7bq" alt=""><figcaption></figcaption></figure>

* _Enable for all projects:_ choose which Projects your custom field should be applied to. If you have to capture the same data uniformly in multiple projects, you don't have to create duplicates of a field for each project - create a custom field once and apply it to various projects:\
  \
  [![](https://qase.intercom-attachments-7.com/i/o/597122376/48f39527ad1a830f51bce63d/cBRX6ILIbVlHbQVRTLJgtS8LPWstXf2Aw2fDe5bdyV9njAeEtAWBXTofFxrMkWVUOhBQk4Rb46lKxBe--E-\_QGO37ki9Y9rwb-mvu2hncitkemCTBt-8vOXkeo6Q9yil-9L8B-sHy7\_e3zDjy-Nl0J2vl\_xahMFn6DgU9IpdI2GpajOZa2ghbsm8)](https://qase.intercom-attachments-7.com/i/o/597122376/48f39527ad1a830f51bce63d/cBRX6ILIbVlHbQVRTLJgtS8LPWstXf2Aw2fDe5bdyV9njAeEtAWBXTofFxrMkWVUOhBQk4Rb46lKxBe--E-\_QGO37ki9Y9rwb-mvu2hncitkemCTBt-8vOXkeo6Q9yil-9L8B-sHy7\_e3zDjy-Nl0J2vl\_xahMFn6DgU9IpdI2GpajOZa2ghbsm8)



* _Placeholder:_ provide a sample value that will be appearing in a field in a faded color, while the Custom Field remains empty. This can help avoid confusion about what should go into the field.\
  \
  [![](https://qase.intercom-attachments-7.com/i/o/597122379/156d355ce5a6ad7eb60d8af7/is-M4QsicDvA1VOyS0OY9VyPrMXwKoR3pvtWciTRyMO0ZKvCn4WFPczaYklL6PBf8x0TWddq6JH02XhnJiNUrsAbNOYvGC8ZoJmv554cC8WmubNy6LlvrqSW4HTy3pbI\_0dxrIWimxePsbaOBzqPSzWbZs3xLjScXV6NWUxxMqTPCjYUoJd2iZTkAw)](https://qase.intercom-attachments-7.com/i/o/597122379/156d355ce5a6ad7eb60d8af7/is-M4QsicDvA1VOyS0OY9VyPrMXwKoR3pvtWciTRyMO0ZKvCn4WFPczaYklL6PBf8x0TWddq6JH02XhnJiNUrsAbNOYvGC8ZoJmv554cC8WmubNy6LlvrqSW4HTy3pbI\_0dxrIWimxePsbaOBzqPSzWbZs3xLjScXV6NWUxxMqTPCjYUoJd2iZTkAw)
* _Default value:_ to avoid having Custom Fields left blank, you can automatically insert a default value.\
  \
  [![](https://qase.intercom-attachments-7.com/i/o/597122384/ffec2876a1267b3644a0c77e/zDhcpR0gW0-dN-rfdAUWVRfXQ4iN5guGdaTBC3t5WsTT5g7FVxpt\_3Fi8RatmlRekswCjpr-KAT7QprR9XkTgCkrp3j1JtQkwr5r69cgzOzogqfxuPIOaDdVIhfgRRTSbjIxm\_s1xVYHoWyRaxOV3Umj5\_tcCUdETa-SVmdW0EVOtOg82UmwTDZMDg)](https://qase.intercom-attachments-7.com/i/o/597122384/ffec2876a1267b3644a0c77e/zDhcpR0gW0-dN-rfdAUWVRfXQ4iN5guGdaTBC3t5WsTT5g7FVxpt\_3Fi8RatmlRekswCjpr-KAT7QprR9XkTgCkrp3j1JtQkwr5r69cgzOzogqfxuPIOaDdVIhfgRRTSbjIxm\_s1xVYHoWyRaxOV3Umj5\_tcCUdETa-SVmdW0EVOtOg82UmwTDZMDg)



* _Required field_ checkbox: checking this box will make a field mandatory; an entity with such Custom Field will not be created until Custom Field is filled in.\
  \
  [![](https://qase.intercom-attachments-7.com/i/o/597122388/83dc4c1c82ebe0d4036c1270/tvGcgVJjwNmSXB0HSzP7dcrRnwF94hNfB3Gz3-T9bZYdL71USdv\_g3fIkU9kLigzXDvHdkuMaz111EiZR-BQhnHXX1Er6UgI8-rlb-Hzk2hG4j92f0N4UpVTIxYvJ\_gz6uZBMe3JmLS9xGO9VKMq9NhjZiBnr1rv0yJVTSKF-sIzSKld2XAZB1bwLw)](https://qase.intercom-attachments-7.com/i/o/597122388/83dc4c1c82ebe0d4036c1270/tvGcgVJjwNmSXB0HSzP7dcrRnwF94hNfB3Gz3-T9bZYdL71USdv\_g3fIkU9kLigzXDvHdkuMaz111EiZR-BQhnHXX1Er6UgI8-rlb-Hzk2hG4j92f0N4UpVTIxYvJ\_gz6uZBMe3JmLS9xGO9VKMq9NhjZiBnr1rv0yJVTSKF-sIzSKld2XAZB1bwLw)



* _Values:_ Available for Multiselect and Selectbox types of data, this area allows you to define values to choose from when filling out a custom field:\
  \
  [![](https://qase.intercom-attachments-7.com/i/o/597122391/ad37ac981d120ce29cccb4d6/tg9gVhonEHzK19lGRhmTMYWx4f-TAavDteVRx9Lfyqbp16Af0bMhwsys-Ej1dwTDCssuR\_3LGkKlDQ86M0LkFe\_2x\_uztpnmuo1sPMEsAQrsjUE5XeUDv4DRvBjvP5zsgpLNTC7N0QJAUD3bOdAhQn0E9f-9cq8jfo3E53JuEC-S7LBnrHpaCtpARQ)](https://qase.intercom-attachments-7.com/i/o/597122391/ad37ac981d120ce29cccb4d6/tg9gVhonEHzK19lGRhmTMYWx4f-TAavDteVRx9Lfyqbp16Af0bMhwsys-Ej1dwTDCssuR\_3LGkKlDQ86M0LkFe\_2x\_uztpnmuo1sPMEsAQrsjUE5XeUDv4DRvBjvP5zsgpLNTC7N0QJAUD3bOdAhQn0E9f-9cq8jfo3E53JuEC-S7LBnrHpaCtpARQ)\
  [![](https://qase.intercom-attachments-7.com/i/o/597122395/138dc94279c12d870a0c2de0/gMlFY3G54PG5g1bMK5P\_v\_BEyfEsVYdNVQLUOxOay616JVi8D7Lc0kys1dDV\_3V19dNJi5APQL4zgVeSN8L8rvV20GTRuAS6xOaXjhPR-3caeFvgCdDQZs9SWkSyt5uSkkBg3jE3XpRhsFpSDxlIXUwAr76Ps3be0MHQoPRXVf8ymTxq0xbzbeyiPA)](https://qase.intercom-attachments-7.com/i/o/597122395/138dc94279c12d870a0c2de0/gMlFY3G54PG5g1bMK5P\_v\_BEyfEsVYdNVQLUOxOay616JVi8D7Lc0kys1dDV\_3V19dNJi5APQL4zgVeSN8L8rvV20GTRuAS6xOaXjhPR-3caeFvgCdDQZs9SWkSyt5uSkkBg3jE3XpRhsFpSDxlIXUwAr76Ps3be0MHQoPRXVf8ymTxq0xbzbeyiPA)

1. Rearrange your values by long pressing this button and moving the field from top to bottom.
2. Customize each value with icons of your choice.
3. Add a new value input field
4. Delete a value input field

\
