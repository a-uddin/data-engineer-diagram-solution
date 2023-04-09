# Data enginner system diagram

Solution Approach:
For this challenge, I propose an architecture that utilizes AWS services to create an efficient, reliable, and scalable pipeline to ingest data from trackman-backend to S3 data lake and dataengineering-db, while ensuring data is delivered within the specified time limits. I recommend using AWS Glue, Amazon CloudWatch, Amazon RDS, and Amazon S3.

Solution diagram is below: 

[diagram link here](https://online.visual-paradigm.com/app/diagrams/?lightbox=1&highlight=0000ff&edit=_blank&editBlankUrl=https%3A%2F%2Fonline.visual-paradigm.com%2Fapp%2Fdiagrams%2F%23diagram%3Aproj%3D0%26vpov%3D16.3%26vpob%3D20220410%26client%3D1%26edit%3D_blank&layers=1&nav=1&title=TrackMan_Solution%20daigram.vpd&vpov=16.3&vpob=20220410#R3cU2FsdxGVkX1V%2FnMDWlrtnVh2CpB5C4iWmWBdBo%2BAZ3%2Bha8vz2Qw%3DK8yIhrR5TW6QbFgWuD1HLd0Gno4h00NBb9%2BsmP4FS2GR2C8%2BK7UvF0TvhtKOGHaeGs4BGJc3Ivtm3pTW2DnVLgYWTD0i7VQc0qGfpYMAJB7rDXKjf9B%2Fm20UFKD7Bedpd0BAWvG1vb0jIozGfS%2BEDmsh1uyhAquRx0FNxmapbJEDZmmnoniaNVNVO9k4bcZN%2BPlYnD3paJQxI9gCRYXYLpbbOcGkY3Eyk0yUj6EZ8RgxbnLqkElHcFRI53cA7YD%2Br59c2F3AwnlNvUAcbw5XciIuXrDbacAoAtYszSeYl%2FtF7aWFMCjV8cf8F7PcLjPYCbHrenvrObifh0UowntQZgYnKZUs3A7akgXR56R0iBEaqGLmrSmkJf0BYrhdLq22LcsuRrrIuxIAhMYHk2Q60Ck6sx5TAWvTj9uH4mnqsfhsNhNq5wqbnxEET4pFd9LQX65FHZ5AzvFAeWerE4KHBl25l6dZIyzVLiM1TmghQPc04hU5lBIQvaZ9LgBnbX2taQ5gdFSzZE8jJPU83HAwqTlLCotVe%2FI%2FHnP847oLqb2%2FjLdsJqOIuczHgBS%2BDzzwl%2BTYpsTRozfeaLUqGVqXiNhKkzcLeEXMkTxt1nXolvU86iwrDORGi%2B3Kf37Ck%2BpJMwcRtoTuQoP%2FzdkGfhOZDWsKoiE5R9T%2FQ9LpbOgxiVuNtrKFPcIIkI4jwx26e26PmurlkV3naoXkWmB5hJZVgbyp8QF8a2TD6yN0Id1VbMpiek3Xq3xhgR99x%2BMf6s9VMKEkJtRCm5ft2GUVOr%2B7so9T2fiys3Ei57hlpdpatnDUgSpGTNcoB6gM83ZJYr4RcJ1TtFXdIGceCkfVcweS7Ok%2F1CQiDoAJ2WydMk6pTVj8s6t%2FmOi503jO8u7A5%2B7ZgXPm4W%2BSQGo590k9zdO8U7QTTiTvzrb7Jh9AFRJ%2Fvk0IGS2nTPDLAzl1b%2FL477JfEq81gYB%2BgTzO%2Fj7yuA8TQJ9KJo68zRHOMo7QfEmpsDLb15YZ%2BbDgdpbZ%2FgsubAZ3W9kcPBVmedzqU30ll7npAycVrc1x8Vdfii5qw%2BkbTKOfVfWe%2BJ5aob6%2BZXuTyJx8raTaWcNBa8r6JJTT32hnKvjwfWOKQ3Yvx892R%2FYoTSWCnJXoGachOD7mG1TYm5sUsLWEkDItu3ao1v%2BYhl%2FqEzzPqRBV%2Fk8%2FuHiwnnSSFyN7bauziYbklAyW4a0VSmHRR9%2B8zXviBkKH0FtHjpfWHClaaVZVIXAMHj4%2FLWpRfJvMKl1l4KV8I2aLbC1a5JOxSUwEmLuO5%2FgYyplMkZNrzeuNAtr0IOOn3uVwQY9dWuLZq83ssfYqQLk8VZhL%2BASxaU%2BzXnD1j%2FfS4zrAJpzCNdut2Q%2FC4R5ffQCbbfW5rTCaXi0wNTHkeXL8RjYU26xDEQHtkMxD8y52YFelTiwj94tymiTFK3xS5u3Egc5I9puQuVAuKsoajPSQyMSwYDukj5aB4%2BudyLb4rVQJa%2BUc6Lu1VoNg7dxaDOsQmLykjSBix6qCEsNVIgEaAqy1WH3acfyO82elMWPEbiBq432gFIqMQf7l3XY%2FyljNYZFSj896tzdOXkyCfAhn7iZ0Pe%2BOrH7yJ733hQNTr6Oqf5DBaQScY%2BCMlsuJhOF6GWnRTni5vyJEE0aDwetb70W5S5JkAy8U4s5ywZeVSzQzIcn1FFjbpGl%2FpZasozPwq5V1TuMIVus%2F5bUVnA16pvDE4%2FZRYQea2cY0A9iKqgbkjBbd8EpBe9il1W%2FKpoUSyIstU8j30jU35%2BReyGJ3RQjKl8C%2BpiiVwJf2B9GqTdDHJUlnyfjf66N3bLS54NWmpx8Rbvafq%2FYxSF513Chu4%2Fr4yzOB%2BTjl4zkxKitQiGysW4MAjFktPpj3j7CJdbji9Z%2Bq7Mv1oWqYYcH7%2FOtFdAgz6%2Ff%2BKGyYqWx9V2yQ12SVix4zJtxAWuF0ZhWpkmsUitNQ8B%2BPtcA9FT5E7p6XvCeZ%2FU9T8t9ljgvVJ28tqzGtCcs%2ByG4qh5SmuXIRg1FGLhjR8nJyGiNL%2FYCI1YkkN7QLeTBhr3bh0RYkITJdIfG6NGWHV1N0wqXT%2BEO7KHy%2BmHqCHJ3Y9JBcy9v3rMX49OA7vwvCQ7tCWDlDoB9n5Z45WYEsUjeicKkuT4Ix1PzhBK%2FZh8dXqxTImyn83D5KPNf3QeQ5ZYZ8uly8A%2FB6bSUANDAWt5qAINk8OUfSDHIPlgZ18zNcnSfObTNiLePZnj9%2FlhpsX6iFqGx0LqwoCyjjb3vUbrx1ZpBUxNhGJKxPuhgFsFrlj6h59nsaXo3nZLvTcHbR%2Bis6fJoJHcun2%2FkNoT1uRQbamwSoEFSHafSc6FFwOgt6%2BKA%2Bhn7b5Eb8BUxh%2Fqu7JmMqkkRrhN2oTKkEjNsiV0lOly%2FFFnY%2BFS0Qe%2F5q6k1jU1GThvPdMRFAP9jiCC4DmC2IrM2WDnJ5u7FGBIhXJW7YE%2BytOPaVOxhgvZbAt4KNMAz8%2Br4iPHpIHSgLb8y6K%2FfpFcwISV8J9AiySCIdQKeCQE0aG8EL29HhJ4PT73oEq5xud7PEhBtmvyBQCLXGgpBXXpBNTvWqI%2B4is5ifx8f1E4yUYLg9ZKMdbR5lDjCMq15o%2Fh%2Fzj2EcFWAanL4s1wLRDmHkM0G4XoEYRW4TWtb4s5EBzKgprUT64i4oiJT1e7V3G1SVhH13n9BhG3kjFUrSfJqnzZ%2BzswPI7mCLWtHyVOL%2BPSUZZQ7UGH%2BE8%2Bsje%2Bxv1PFfTHM0vLroh749o2GtObuBWlAwotUb1gdBZNNeMsUkGqOyVzPrydFheEIDx%2FSlQ9fWagxQ0te7U1aWyfRSvj8JrbgtyAyaPQD%2BMWxwThAGt7MX4YADD5mL8%2Bo8zEISuV7YpPwkfBdGx3mNl3Zuprz4EqWxn8HXs8zVxs5U%2B%2FdxrVX7zA52FYM1J0SSKVxeK7OCpnwKo1zSFErAC354bJCFvyGrQYWjFiaCdY5rBerIMBoonIF9W7HMUV175eETJz9SqIthp02RpoDDHT0NBk0fvAXrBojrSn%2FGiKwEtNpmMG8zi0RqQyMl%2BlgtjeiX2fTliUnkonuefhZXSWsWHtHMaFJce7YRMaBrsBGDISfg22FJ4j9GbgnOYDMmVwFYddgT1FmObxPoIT%2FdSdYlS5dg0lvaq%2B5HXJXNk9VZ4utDBWrhEKWbiRVxZdctxPKN7Ti2k7R52XAGPN4a6jOx4s2xev1oqI1IypVg4dOD9krLo4SBgteeezbaHVDKMICrR4DNp0SiqwJR9IzQAN%2B6mpRbzZN3I13qE3FrN539L7NOg2KMTna%2FITtpw5yTWuT7LP70GqpxLo1Sobq3dfSeqkbzAKTdI702Han12%2Fi7GUfncCf%2F2NQbk5TwQRJGni0Fr2iSPA%2B2F28k30RUX9kqQaKfMcMYj9DctptV6XYtRCX8e7FH0ruJkzUkv%2FEe1X9kChlMHCfDm%2Fh%2F19BzYH%2FPAdAAmq4nM2zlLT71pxD1WX3sSSrDCe%2B4WAR1GHl%2BNRV0gEQfkGWPc%2B9ct5pfLBrFYgSjZkR4kmpasPaXb1KJzdT3KS878nl9OTcHzegwuvNHWicDFvU1rwHpqK1GY%2F%2BoTwSidQ6vQqTXl95%2F5cacTAbLKQ0%2BCobZDr8bV8MQ13dfVAQPrqcrBtvCx4QUMMaVaIP9U4golnLCATq6WBthwc6MAaoWQDLuv3Y5E1YTJzJ3SpdiWurbOYZ2i2JAnTEfEIL1NUFJo5dXjLeK6nxnSXny16ITGUU97TGyag8gw8Lv83IVEuA366JwUCLX2zSoHQEQ0nwM1%2Bt0uJWQbPSn1wVs58QDQ3Wg6HHpiUHyujcNrZyGm4WzQ3MYFCmCIGb8sdENL9pJWBbbsEqpbuIC5d4CoTNrCqkaYbGfwnBub69uTfycNkRfPcZ21XUvDFXBN1h6HVIDfdNkgrSTBSY8yt%2B4fJdexxlwqVBrDbLCve7anDqHXfVs04DcAaXfGmeSfjPxzuDXKUnVCfgtE91qys7Igrg9qpm2Ugi%2FicjOTNYiDyeE7%2FoIeaiekw5bz4btq5Z%2FEhbNurktTFNDDU4zKSa9Rl%2F3rJJRyW9MCWrW4LfjqCyxBTaGCTFZMc0ujDfjvGGFbQWu3jOR5z22FvMtJlH3db56pgnDqciljmp6MR%2FXjl3BJmqjeksQ90iW9YPWq3fYlnltappJIhheWUn90MKWUJ6mEkJHj4HME%2FEbUUcX1dfdgi7AJPtZpd4dPJmuzKLRETd560VvSDxks1iLcNbuVBdOOgltM7b87oHbbzqbsCX4beIDiIJ7M%2F9QVLgPnGh54wrYAc7iOf7lTngPLAiz9G8T6af8j3g9QWivVnQuT2NiwhQnooWwps%2BqYgdbpxo5UROcPNRrYgN%2F0t2SpAZHRjIMq06qC0FipX6IFpYgeUQ7QiAnyrix%2F1ZQrinE1XtBOcLtHwmgQrEyMksqedprTuAWTZT65mNfMmplWlYWtuNDTb2vwW4E7fL1uGiX5%2BK%2BuLwSdiDJ2%2BygzVlv1jNo5VDfeFQNG4iRmeymshbSIufQxOGtwu1d19nW9yvGeSNnnvnE4nJvyrmdb0x%2Fn6xCJa%2F63DOHAvLZCs%2FQ74v3P3h%2BjVevA9MNz0UYeYF0xq7GPvtVUeUdMoJxgWMDLsps%2FP1LsTQuaYzl%2F9njB%2Bw4fbRaVOQvv9qeOUQerJAcofuUFslAKBzQWaSo0407%2FhV7uSEN8EYoztQY1MhrZ1yh4XMbrvx1zqJGSQxR9ymZA63L%2FRV05XGlMDHv%2BbUplroyKJ0qrfCyhLDv8ttyFT2Iyo5pajTFwm%2BuqX1BGL6ZM3rFfBccdKaOJZ6%2B9K4q%2FOXT5PbrZFRFV6dIBFYN33%2FbPnEv0MGsb4S29WokZIOMIPTGL%2B80brQ2zXziAcVTwi5E0bPVz%2BzalvkMoy1Jv619sEN9wV0XI0EA6wUYGcqSyYPCTVx%2BSvE%2FFPMi1H6WEcoCFy7JAWfB8lfLA06MzHSMpGX%2FP1dlwwAn5ThBwUauTvDStKIELZ90yEfeIh50bpVXX8ZMYeLN%2Bjqx8fM4AKmRtL8g%2B3xvkfhdk7FpFQh89afQ59zf6tYZ3FaH4AiCbGU4%2B1FD26iQHvOjd%2B4PLYt6gHXzDm%2BRdbS%2Btps02GkNBmAAPiF0C1w0N%2Fai5Y1UYvhffZWN1KGRDtjTgQesHik%2FPWtUA9oemec2KQYOLqSZk77KfABbaP19RCwCudZmp%2FZDxqoEEeDzM8t44Gc1uhfKAysWtJNfBpOZkjekGF%2FHmMpq5JcwNbHtQEuxgcx%2BSlD42Zo7vhluX9gSkGG3a62p1NU7tRJGeraWI43%2Fs22vULQq5Mi0yWuFAxWIHRF8EKptm%2FDiHQX3Bvp%2Fceu1fBNLl0crx8fDT6%2BSKaMX4HznEh0Ulo3ZnzDic26rByhLBR%2Fk%2FpvwxAlmodKXNSRsOWsHE5Z94prI7DIQTadZUbbJTqckwcTAsLaLCrBvTQ%2BYetRvWGoHgRwcWpOSbxedHVFnLRuCcrrUElNEggCSneV81KftfyALs70KqUZLj5Pg6evQ3ajPcioCvlq%2FRoRyjg8mmssnWo%2FAZEq%2BBCs1xnhaT2SVFb19fKW1y9h8L9D8JH9y9GKbL%2FaMDJbd%2Bp9aiD3DcU3qrIzNk7fjG1l2r1f%2FouTkKXQ0SjKdtmKUZ%2FXTYwHB%2FIfPTa6NCQcPmx41YLiAbJfZMlg8YmffJOuMbgi3yGHYL5JUeGKlopFGvqebhcQM0F2DllagYLjP7JESDwA0PiVz2sRVgs7Vg2kRRGz66%2FANn7mY%2BjWzQOUcQ%2FDVFicmBTOO3XDTh1PYlBDutgCnBsIjqB5Zn4TVZijh0lqdH6isjR74QbxdtxlbARJB6RDZ9Cirw%2FmIHQiNn5C7vyvpbrrt1tBaWTQN9%2BoKrU8YYdAXMSp08Lo99qV8eBrnyFyxjY7cbJB%2Bil%2FFVCDVR9l18UQi46H%2BnjBdJzTv35q57IK9kbDX5NiB0PTKehedOEC7MjN74rrgcXttSSJ%2FhiOB384GN2YCusO%2Fa%2BEr82oGtOPCaiCWAresjM2Nj4pzjns4nR7X2Cy%2Bz0vJpAEA%2FsOJfIyaZvei0ePJaP7XYtxWlmY16pHQA5HLXb2Uvd2n5X%2FRkv91mfEJbt%2B%2FFJ5rPmldhaNIsxJT6EuZnZW4j8eoM81cX%2BqwRFaJkpt6qDouR5H4U7ddl2YqgYmyl7FiDDvR6cKpGntEbzaxruEC1qOt8ls4xUL1qF37BkEkQYw27Y5fYJb8FxieA7q5PpGnHM6KltC57vOsadTgM7T9WQUn6GQmFaQFfifuWxHMGPxdftX462ZuKEEWr1NR%2FTDL5X83HeF80SZemjofUXE1buz6d%2FqkDy%2FKGatYRkLVYOo%2BSUWjwFyEcv%2Fyp8aPvaYacc4z1vAnNQzlQ9pk0S9YzpaobGoSuWcoEFbJVKBx4HEa%2Bs%2FFF7FGb37UMXvZQXgaE9LAud79Zjk4StpCVW%2BfYL%2FBhLsxt4bIuUn%2Fj6qKMR%2FRMHfZ5IPIjGLK37LLNua%2BaLHDo%2BxNAf3vGIgaBqFCei2JTlk%2Bi1Nz5gvnVDAOl5ajXZHO4AJ6MLpAQivVRleJOUZ%2Fp6k6mGF7QWp4iTuNYjqwCbiXoYsiTTM8uHYf8l2H5BUN7OkZ1Yg2PMf4opkTVy8j%2FnmbtS3nWsbxR0pXuqhJj%2BTjASkcG07iEtxlESCUrsDSfTIc4ZXUGDKhpA6bxPQEB78cfqwF94lJpqBK9%2FGDe2o0CpoARgvGxnanCOfDImDtb0YcHsmSsNIO5aObeRjBe6NqFcdhExskhGGtQ8hYc%2BjFqTIptZmXURlfRhhQY1wrzjyDKmi%2B%2BYjYwJsbHN1NZnxhQJlRwGdTrpUptKlZNlii1m%2F7LA2jmLEnOv%2FS4tiHQ04oq0cB5EBgxO35bgRp%2F%2BaMga8E8Abk2j3%2FBqkjPfwwYyvAGhUUWvzw7wGqrwpZfl3Ui6P7epguQIdBBRik5ChH%2FRC2IR2PMymay%2FHkiPJHQ2gVtg32H3ezTh2e22wc1QJfRtKra3X0MA6q2EVIyib5BF%2B7lDjNc5ai%2FKtt%2Bn2AMFJs57iu%2FyIWqTTTw7gWGrLug5od9GbGx4%2BaNBqgZL4yKqWz7QviX5Jv5xz67d0sMttlI6hfK%2BZl0nldV50l%2Fgr1wXSx2U4mVSZXOrbigZf%2Bo3dFCQoRYMqgSMsOKV094WQl7oJXXiRsY1twiEhd1x7UNlGtBr%2BbNXaQ%2BnJ29uTg1Q8n%2BToJAYyZDKUbpcKkmqtoueD%2Bj%2B%2FuNDJ3cVCKbdVdqeG%2Fs6Or0EwnSHuoeYNwjLjkFZo2xjItb%2Bj0d2YKtBjdRXQnthQmTtrHeC%2BVvR2wZan%2BFPgwE9OQsGgdIKRO%2BoAfdMNWRaZWh5NTdfZOb0GppE0qZhws5vOgOeTExQ%2FDkGw9rqOvlMBGVyxdsKYACECkVDsL2o6Xrdy4gPfdrTyOxOUitae9KZEEXqFRj1c1XgNlKSLdjdFfyuKbkp386PmjtvSKCe8UERldWPUzGQChuBaBm1FMb9WNz5j4vFjCkjk2PpMDw%2FIYdtDtDNzQFTwzOBaapCkan%2B2EFxW%2BcxpQr5qwPWMA%2FHh%2BnlE5KUwOSdkUsfIZN05cTFV%2Fb%2BvU4VEc5eNbVxVl4C3GwLPJvOS%2FBVMsnK6XkUE4luHOP1XuxwP7OVaRoHq8SV%2B1sV14PmDYAuUZbLU0yAwdS5NO3R5%2BK%2FAVBWgCcFlDTk%2BzAOorYdycyXTGJoyFibV%2BR68oypdxdiOjPjudSprriqfueitP4ceC9III%2BnCLfCVsCBhU5yVQZt7lA9r5GNKOsnXbWTxKZHUqz2Nkq6RjaaVdWrb7LdK3n%2FKwwB0KKjLIaHi42EozsSD91KdmBMVWpOT4kEFNotwLL6gRTz5ETLdc%2BocvymyS7zrDFqupI0gm0SyDq4%2Fq95dMGU4jPK%2BmCbKJqYkONeszqPj71JzGO8vR2Hiy67oTbcsFW8IZ8Bk0MSLh85I7ZdGWM6XMj%2BDPdnHuYg%2BdEposiFiLGIyeGLRq%2Fmm2%2FcVwhyFR2KAkiE58Qm0YWVpAPznMo%2FIUL5DqMdq7lDyiw9g%3D%3D1dVmG114)

Components:


- AWS Glue Crawler: 
To ensure that data arrives in trackman-lake no later than 1 hour after it is first inserted into trackman-backend, AWS Glue can be set up to run on a schedule (schedule crawler), such as every 30 minutes, to extract and transform new data. AWS Glue can also be set up to monitor changes in the source database using change data capture (CDC) mechanisms. A Crawler can crawl multiple data stores in a single run.


- Glue Data Catalog: 
The crawler writes metadata to the Data Catalog. A table definition contains metadata about the data of trackman-backend. The table is written to a database, which is a container of tables in the Data Catalog. Attributes of a table include classification, which is a label created by the classifier that inferred the table schema.

- Glue Job: 
Glue job encapsulates a script that connects source data, processes it, and then writes it out to target data store. Typically, a job runs extract, transform, and load (ETL) scripts. Jobs can also run general-purpose Python scripts (Python shell jobs.) Glue triggers can start jobs based on a schedule or event, or on demand. Glue job run can be monitored to understand runtime metrics such as completion status, duration, and start time.
Glue jobs get data from Data catalog and targeted to S3 (trackman-lake) and RDS (dataengineering-db) 

- CloudWatch: CloudWatch will monitor the Glue job to ensure that the data arrives in trackman-lake within the specified time limits. CloudWatch will be used to trigger an alert if the Glue job fails to deliver data to trackman-lake.


- RDS: 
Dataengineering-db is a relational database that will be used as the backend for an internal application. AWS Glue will ingest data from trackman-backend and store it in dataengineering-db.


- S3: 
S3 data lake (trackman-lake) is used to store the ingested data in a suitable format for future use. This data can be used to create a data warehouse and make it available to analysts for reporting and analysis.

Notes:
- In the future, if we want to ingest data from some other data sources, we can use AWS Glue to extract and transform data from those sources and load it into this data lake.
- The data in the data lake will be stored in a suitable format for future use, which will enable efficient querying and analysis of data in the data warehouse.
- Amazon Redshift can be used as a data warehouse to make the data available to analysts for reporting and analysis. 
- For the query we can use Athena.
- We can use AWS CloudFormation to deploy this architecture, which will automate the provisioning and deployment of resources.
- This solution is scalable, maintainable, reliable, and cost-effective. It can handle data from multiple sources and can be easily extended in the future to include additional data sources and services as needed.
- With this architecture, data is ingested from trackman-backend, transformed and loaded into dataengineering-db and trackman-lake in a timely manner, and future data sources can be easily integrated into the pipeline.


