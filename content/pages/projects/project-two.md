---
type: ProjectLayout
title: UNT Search Engine
colors: colors-a
date: '2022-12-03'
client: Collage Project
description: ' Led a 4-person team to implement a search engine using Python''s Beautiful Soup and URL Parser packages, based on Vector Space Algorithm.'
media:
  type: ImageBlock
  url: /images/bg2.jpg
  altText: Project image
---


All the required packages have been imported which includes the library to fetch and perform URL Actions(urllib2), for parsing html and xml pages(bs4), for performing mathematical calculations(math).

For crawling the UNT website a list is taken and based on the depth variable all the sub links are crawled. A library called Beautiful Soup makes it simple to gather data from websites. It provides paradigms for iterating, searching, and altering the parse tree on top of an HTML or XML parser.

The URL is first opened if it is not crawled earlier and then read using read(). The urllib.parse.urljoin method combines two URLs—a base URL and another URL—into a single, complete (absolute) URL. All the corresponding links in each main page are found as it looks for “href” tags in the html page.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXebufdQBV5U9BQdp6DOqU4y49vBdDRBHan0iDjM9u3s9cyy3b4O6pwNZgY7xPCN2cEmGEZqkKfZi7vFGVWmd42mLo3BYnUClW7_QxLLKyt4CIeofcYWYDv2JXV0CTRc63IyL6kb7rG8jfpIzZICnQBM2GW0g9o4QODVn8pscA?key=d6wXEPP84P96gtjLJFjnZA)




![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfDBAMGS9xIudehkSMpsfBRkVm_LsWWBE-BnX0wfc5FMFUzJP5w0TtQ2uCtFHEAp1Yy3tMtbtFnCIspVDk7u8HkntwXjAPFoL1pXLGgRjiVCZXb5HDya51PQxWSQfFt7458FTAfBGKaXYcszRPdTmfCEGic7-6X1ZzueXiZFg?key=d6wXEPP84P96gtjLJFjnZA)




All the pages that are present in the UNT Website that have been crawled based on the depth is viewed as shown below in the form of urls list.




![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXddHmLOMGJrlXGmL3VpECdf9v5Cp1PKIjSmuNNayc0UCJwTE47Wa0dR852MoTsL8Rmi27f_p51mQJ0ToldSODAdI1bIBAqxPYOBxBlZJA9kCRTAXxf1TKpbGeQUGitTWaP22ZhVNVU_MyiJvZddZ1JnbAEiTWKXiXnmsZPa?key=d6wXEPP84P96gtjLJFjnZA)

A unique id is given to each page as a key value pair in a dictionary. The current page is obtained from the get method and response.text returns the content of the response, in Unicode. The entire textual data present in the response object or the webpage can be obtained using html parser followed by get\_text() method. This returns the whole text, including any whitespace, underneath the element. Hence strip() is utilized to remove leading and trailing whitespace ().

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdwv0H7zRBuX4K9zf9Pll9A19S-0vxLZa9KDpFRykdMJpz9RYj3sNZ1-866hlYAaYY9RPUY4jIB49vMsfI_sBfJ9njP45E0WlSZF1Y9MuOrNZAMMMc6tlnKGYRNSQRlZKTDVQeK4KoBCOy1g2o9PX1ahmJMN4RPMAXI6mTFeA?key=d6wXEPP84P96gtjLJFjnZA)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfpzsg3Pw6noQgVWatWhe7C92rRqMJUQXGNyZ_arFgjEa7Jd-FUmItTItUftV8U3s0oMNwcSmghIl8oT2ZOXCAhATxyU9shANuFJIsq0QHrOoet5xzMso2guqAN-9VnzGfxuguNBPdfC44E9a1j4Ovur2_uKKTeMWz-YGlulA?key=d6wXEPP84P96gtjLJFjnZA)




A directory is generated using “mkdir—make directory” command so that all the crawled webpages are stored in it in the form of text files by writing their uniform resource locator addresses in it. The function downloadCrawlPages is called in the corresponding cell.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeNJMb3kdWDMtMPkVfSZlLOhoKApC63OXsLcts4dsQBoP91Ez6GiYx9zZFS-10hRSollE0HGsQt7Le-PzJ5HX2POlUJ1SgSNdM8fMIKZVq9QAvpf0Am8zGL19h9JNDm7ZLn0mwkZ9xzsy-aQocZuYHzdu_zGphK0ya6zuLmgw?key=d6wXEPP84P96gtjLJFjnZA)

The score for the relevance of the document returned based on the query given by the user through the query id assigned, is calculated. The output is written to a ResultTable text file with highest rank and score retrieved first. The inverted index is constructed based on the term frequency and inverted document frequency for the queried term. This requires logarithmic functions in math library. Cosine similarity is then utilized to determine the relevance of the document with that of the query.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdGf3EGRVt3VhgKavpt5Mda-PpxkW_UjQbjVAdytoZxT00e4-4iGHejM_pJA7HHRntAm7eqdQy1xMZM6NsS8iMS_ByM_2vdZuYc-eEnvqH86aBQrFjEp84eaOou4L-ffCZz5TTtWMn0THaOHDgS_PwLJIkTi6WOoihhpqWQVw?key=d6wXEPP84P96gtjLJFjnZA)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc5jih1Zdx1XvGiqb8aduTBOii08vsRAgZSzX3mXCTIrufVOvPZa5BFrO4lEWMxA9Ahgp9LcAEtrl9ggXeGBaYyzxGd7Fu9Zt553rLutTWYcGoVvCXalhkzMtUux7wSkF8v67CEanpIXo_I3SGE389YwjL_oFxC18H4DH_IhQ?key=d6wXEPP84P96gtjLJFjnZA)

But for this, all the stopwords in English language such as “a,and,the………..” are removed by first tokenizing the user input into collections of words in lowercase. This is done by “eliminateStopWords function” and is returned as filtered\_sentence. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdTsA7hqX3dy5Ng7jAN-H7a__3Br7Hlfkwjv9GPxhcdUYkG8jIhdT8f1RqGuPt1wDBFJESPovbHYHjO5XXLWQSNdBaAHe4rOwnBSMfRacr3zqt348G8vUFI2A-cx_FaTpJMGKOxc9SrN0gTrRbLqlMtvvEnXtuQtQQaE8p9?key=d6wXEPP84P96gtjLJFjnZA)

These are then stemmed that is root of the word is determined. Stemming is a method for eliminating affixes from words to reveal their basic form. It is analogous to trimming a tree's branches back to the trunk. Because of this, the root of the word is recorded rather than its variations. Stemming reduces the size of the index and improving retrieval precision.




![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf49eyGULNkgsppKCWFD02Cj8qYFx0uiiam3ZN50ndRxoaMCbSejy5Ekuc-scg2YCIcCFxvI2nQrkp4lLhW2qQqPVLNrPEYKCath4KaKyeqtpCaQG_nHXf0vuZSY096bTPIlB0WIMYbKAvOxXgvt32ulQWxFuLOyAWQYZ_O?key=d6wXEPP84P96gtjLJFjnZA)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf2uBMqM-XB0qQkFAfLs32Wm-tQAbumdzK9rvuX-jBKgbOLnT7twhp7rLFRvQtL9yLgS_tiqISnE4Q5oPO5klOSz164U0_mMedX7Qzl3RAO2JsCdWjkHq2dZb7loPeq4E16azAnDkD7ikK0TXFjTMg55Mm6AxeYQ0xG32bFYw?key=d6wXEPP84P96gtjLJFjnZA)

The number of documents containing the word that is in the query is used to determine TF-IDF but, we take inverse of this term as most commonly occurring word is given less weight in comparison to rarely occurring word.			

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcCYmYnc3oBYFauGpeBKyEENpntaswUBrlE2ia4YY9cudDSri0Ufu0oi2qEbMbpzITBRcmenygMIaq_AlGKbFzfUUPStAGWbR9BgWI-EOcW4swl6tlnjbI-Q2Hnm1N0PbBbbU6qtALYI6Krii8nnytr_zp5fC0koz48AYHP?key=d6wXEPP84P96gtjLJFjnZA)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeYo3y7t9XMV9Mq0C9KeTl4hdBvSCC2Dt2yDw_oiCf_spodRtzvfkdfDyxC2YacEFe6ai1ER0eoQSiYvJF_D0PR7IULlmN7W7VIISmL8VO2F_b-EoWiY8mxugXg2KS9p3k0Y4dwC6HmLAGHseFrjJ60yL1NVw5zDkEuTYnZ?key=d6wXEPP84P96gtjLJFjnZA)

 ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfblxOQjZUlRSnuAqygMz5i88g19HEX92yVdr9Vgkt3J50eQffoaMTWPg7gjCI6lF7jvBraSHr4Grz4UpooEhf3yRHwCF5qAAn0fxA5UytnKKLWV01UEf6ARdVhanI0A7fdpBiKYto5KlJEavWoRVOGNAEnxT79EgzqNA9f?key=d6wXEPP84P96gtjLJFjnZA)

The document's score for a given query is computed using the cosine similarity between the query and document vectors. The top 100 documents for a query are chosen using the obtained scores.

				![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd8m7VHd9T4wgoZgBFCi0t49rsdC2lMzU_5R4h_jWbYm5-OAqPBh2f-cNzNw6bEbDabxgTNqQPToRLk3yihSVGU19MdgHmxUEuU753MNWc3LFHPDduhpbmJh_v524LWMm4gx42jLbLdUf6DngnKr-aGFctZfkU2hxDzEJMx?key=d6wXEPP84P96gtjLJFjnZA)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdIA0VRtYCcnAKKbLugQD14BAibpcQFz0_SNOPhoTkanPdEjDHrlbdpqMjtUZRbEk_K_S-XvrJTb04CbkoReFjb7qspw7Nd7ry1_By9hDLpM2MN2sIYS076YiaObuwyRtC9Uj-ZbkBCNLz62Ovg5tjdDeqx8oOYkZG6V8-dKA?key=d6wXEPP84P96gtjLJFjnZA)




![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdFwxTSSu-obre97y5rprC08iheql6PgJFkpseAbZ_0JPDW3AfJYc1LUoaMkgMPpFmfSu5wwu4HAdCApbUkYf0FWqZ0gNK27ksf_OPVN2LEWfGMrpjoA5fRLxGgUSp5Vn3iPs7REZlbGunUeEtJqAuSBidWk4HEOvvI-SX7vw?key=d6wXEPP84P96gtjLJFjnZA)





![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeafYaVI5e33QWzzcbbCRCMyzHwOF9-vAUF_btEs81LtkkDE1PirO8rC2vvmsINOjnrjsrWHY-q_RJbYlSgvbWX8Em5yqouwCHGzX-WloSSjljPSx7TQFc_4uifE3j-HRq99AzUs6j4F6hDQt5EzVxGkbK86XL_CbQhx3U9Wg?key=d6wXEPP84P96gtjLJFjnZA)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdKZ6m6Dauxqap68aa0n1Q1wRw2KOCvAAr39al3DfwznCiv3wBXad1graQ7Fg2VxapjPJnjrZbjOhtn6bgBNntwwsZov7gjK610O3rf95mjQYI1ZRAGeK1fN2-4YweJOlWLr_Q7q7Ft4tyNIfPYurtfnWRmDDfqecXOAVF76Q?key=d6wXEPP84P96gtjLJFjnZA)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdB6TUHBOnh5DrZsBVQXwsQ6AWtsmJQBxlJ_9lc7nbQwRUjUb7Mqx_ZfcAuAt6tezjw7mML74oSTxVOqNnA9ACfE7JJ6WjbvFQApqcraTgTjL2ORK_ikz1weQ9ELxLKUjzfdivmUdOyXKcrZjiUdIfmg_bE31l2FGkeqPmDxQ?key=d6wXEPP84P96gtjLJFjnZA)

OUTPUT

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcstqiswIoZ729-EfpzUHk6-H5Dk3hoplgvW-IlibDDDszatWnXdtcBiPVODrtL3hz8zqo_MfLFZ0PkIK_IhEW0taOCNK2DXZoMr82kJb3aEuv7BmFo6_t7hFUdpZpx1RI818C9PrtNqeU4o49SlPG30jCWtbw52S7nhHqDzQ?key=d6wXEPP84P96gtjLJFjnZA)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXejF9IgffrPU9DYSaPtNGOB9Sx2tQ3EZx6WUz0riEJKvwEwoHQaz0O6hz2eWCXmQxVuxc9mOuEFmbX7UE_N3KMpgZb_cKAbLHCmKmLSV6Z3z8-KRNpiFh7gcnBPAlIFdW5nQk-QIlmht_sP2_FHHvKO9JdiDvnc1anjFAFZHQ?key=d6wXEPP84P96gtjLJFjnZA)

When we run the same query in UNT Website the following links are shown as obtained in the output above by the implemented system.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdygvu5wIhPFi_YQPly2bmZDFqohLNnHX_wZGUNJMTOzkQCbpD7t9fthYMepgQl_L7d4vz6jlL_ZeiKLzNGreF0HyJqDMrhiw2tsWeZNZnTtf6fR0MY84GInPaJEDoUKa0C3oTD4m-I0_nqLUIDzeUGVA2PtJPbaatB_mE8?key=d6wXEPP84P96gtjLJFjnZA)





REFERENCES

<https://medium.datadriveninvestor.com/tf-idf-for-similarity-scores-391c3c8788e8>

<https://irthoughts.wordpress.com/2008/04/21/vector-space-models-and-search-engines/>




