# Lingala Translator Project

## Introduction 


Language technologies such as translation services, speech to text, and online educational games have the potential to greatly serve the goals of minority language communities through supplementing language maintenance and education. For example, indigenous communities in Canada have a shared community interest in language maintenance based on teaching the younger generation their heritage language to keep it alive(Littell et al.). A paper by Littell et al. details how various forms of language technology can be used to address these needs: https://aclanthology.org/C18-1222/. We aim to similarly use language technology to address the goals of a community local to Urbana-Champaign, using a community-centered approach to develop a solution that carries a positive impact.

We focused on the local Congolese community because they had been open to engaging with researchers from the University in the past, and according to PhD candidate Williams Asamoah Frimpong, who has worked with them as a part of his own research, have various goals as a community that might be benefited by the use of language technology.


## Community Expectations


We were able to contact a member of the Congolese community with an active role in the community and several connections to individuals via his role in the Church. He shared that better translation services would be beneficial for new members of the community who don’t know the dominant language. This project would involve a speech-to-text task for Lingala, and then translation from Lingala to English or Lingala to French. 


## Prior Work with Lingala and other Low-Resource African Languages


According to Mr. Frimpong’s work, the Congolese Community in Urbana-Champaign speaks Lingala, which originates from the Democratic Republic of the Congo, French, which is also prevalent in the Democratic Republic of the Congo, English, and Swahili. They use these languages in different contexts, with mainly Lingala being used in casual day-to-day settings, and French and English being used in more formal settings in the community(Frimpong). Thus, a lot of the language-based services would be based on Lingala, which has very few online resources (corpuses) for natural language processing tasks. Researchers who have worked with Lingala also face this issue and have discussed ways to bypass it or to fix the issue itself:


#### [Pretraining Strategies using Monolingual and Parallel Data for Low-Resource Machine Translation](https://aclanthology.org/2025.africanlp-1.6.pdf):


In this paper, the authors identify pre-training methodologies that allow effective translation for Lingala that can also be applied to other low-resource languages. Their methods involve adding both parallel data as well as monolingual data to the preprocessing step, which increased the accuracy of their model.

Another thing to note is that they use the AfroBART model, which is another version of the mBART model that is trained specifically on data from eight African languages, and performed better than the mBART model on this task.


#### [LiSTra Automatic Speech Translation: English to Lingala Case Study](https://aclanthology.org/2022.dclrl-1.8.pdf):


In this paper, the authors define a baseline for automatic speech translation for Lingala, as well as provide an initial dataset for completing this task that is based on Bible data: https://github.com/Kabongosalomon/LiSTra

## Code-Switching

An important factor to consider is that individuals in the community often code-switch between Lingala, English, French, and Swahili. Thus, the audio that is being translated may not always just be in Lingala and instead include a mix of these languages, which would all need to be translated into one language. Language models are able to identify semantic meaning in natural code-switched data similarly to how they would identify it in monolingual data. However, we do not have parallel data for the particular code-switching that this community uses, which presents a challenge because the same researchers identified that language models are not able to similarly apply to synthetic code switched data(De Leon et al.).


## Future steps

Ultimately, the goal is to produce a mobile application that can take in audio that may contain Lingala, French, English, and Swahili, and translate this audio into text in English or French, as desired by the community. 
In order to achieve this, we will first need to create a translation model and a speech-to-text model. Finally, we would need to incorporate these models into a mobile application that the members of the Congolese community will be able to utilize in day to day scenarios.

### Papers Cited
Frances Adriana Laureano De Leon, Harish Tayyar Madabushi, and Mark Lee. 2024. Code-Mixed Probes Show How Pre-Trained Models Generalise on Code-Switched Text. In Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024), pages 3457–3468, Torino, Italia. ELRA and ICCL.

Idriss Nguepi Nguefack, Mara Finkelstein, and Toadoum Sari Sakayo. 2025. Pretraining Strategies using Monolingual and Parallel Data for Low-Resource Machine Translation. In Proceedings of the Sixth Workshop on African Natural Language Processing (AfricaNLP 2025), pages 31–38, Vienna, Austria. Association for Computational Linguistics.

Salomon Kabongo Kabenamualu, Vukosi Marivate, and Herman Kamper. 2022. LiSTra Automatic Speech Translation: English to Lingala Case Study. In Proceedings of the Workshop on Dataset Creation for Lower-Resourced Languages within the 13th Language Resources and Evaluation Conference, pages 63–67, Marseille, France. European Language Resources Association.

Patrick Littell, Anna Kazantseva, Roland Kuhn, Aidan Pine, Antti Arppe, Christopher Cox, and Marie-Odile Junker. 2018. Indigenous language technologies in Canada: Assessment, challenges, and successes. In Proceedings of the 27th International Conference on Computational Linguistics, pages 2620–2632, Santa Fe, New Mexico, USA. Association for Computational Linguistics.
