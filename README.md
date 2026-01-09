# Biased Tales 

Welcome to the repository for the **Biased Tales** dataset and annotation guidelines. The dataset is also available on Hugging Face:  

<img width="40" height="40" alt="image" src="https://github.com/user-attachments/assets/899e6bc0-6ebc-4a26-8c36-b46ded291445" />👉
 [Donya/biased_tales](https://huggingface.co/datasets/Donya/biased_tales)

## 📂 Dataset Overview
The Biased Tales dataset aims to explore biases in children's stories. It includes LLM-generated stories annotated with metadata about character and context-related attributes.

## 📦 Data Format

Each record corresponds to a single story and its metadata.

| Field                  | Type        | Description                                                                        |
| ---------------------- | ----------- | ---------------------------------------------------------------------------------- |
| `id`                   | string      | Unique story identifier.                                                           |
| `story`                | string      | Full story text.                                                                   |
| `number`               | integer     | Story index within a generation batch (if applicable).                             |
| `model`                | string      | Name of LLM used to generate the story.                                            |
| `readability_fkes`     | float       | Flesch Reading Ease Score (higher = easier).                                       |
| `readability_fkg`      | float       | Flesch–Kincaid Grade Level.                                                        |
| `readability_cli`      | float       | Coleman–Liau Index.                                                                |
| `readability_ari`      | float       | Automated Readability Index.                                                       |
| `aoa`                  | float/int   | Approx. age of acquisition/target age.                                           |
| `role`                 | string      | Role of parent if included in the prompt.                                          |
| `ethnicity`            | string      | Ethnicity of the child if included in the prompt.                                  |
| `gender`               | string      | Gender of the child if included in the prompt.                                     |
| `religion`             | string      | Religion of the child if included in the prompt.                                   |
| `country`              | string      | Country of the related story if included in the prompt.                            |
| `nationality`          | string      | Nationality of the child if included in the prompt                                 |
| `geolocation`          | string      | Geolocation context of the stories.                                                 |
| `urbun`                | string      | Urbanicity context of the stories.                                                 |
| `social`               | string      | Social/socio-economic context of the stories.                                      |
| `protagonist_attrs`    | string/JSON | Attribute list for the protagonist.                                                |
| `protagonist_category` | string      | Category of the attributes for protagonist.                                        |



👉 **Demo:** [Biased Tales Demo](https://donya-rooein.github.io/files/biased-tales-demo/index.html)



## 📣 Citation

If you use Biased Tales, please cite:

```
@inproceedings{rooein-etal-2025-biased,
    title = "Biased Tales: Cultural and Topic Bias in Generating Children{'}s Stories",
    author = "Rooein, Donya  and
      Zouhar, Vil{\'e}m  and
      Nozza, Debora  and
      Hovy, Dirk",
    editor = "Christodoulopoulos, Christos  and
      Chakraborty, Tanmoy  and
      Rose, Carolyn  and
      Peng, Violet",
    booktitle = "Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing",
    month = nov,
    year = "2025",
    address = "Suzhou, China",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.emnlp-main.3/",
    doi = "10.18653/v1/2025.emnlp-main.3",
    pages = "52--72",
    ISBN = "979-8-89176-332-6",
    abstract = "Stories play a pivotal role in human communication, shaping beliefs and morals, particularly in children. As parents increasingly rely on large language models (LLMs) to craft bedtime stories, the presence of cultural and gender stereotypes in these narratives raises significant concerns. To address this issue, we present Biased Tales, a comprehensive dataset designed to analyze how biases influence protagonists' attributes and story elements in LLM-generated stories. Our analysis uncovers striking disparities. When the protagonist is described as a girl (as compared to a boy), appearance-related attributes increase by 55.26{\%}. Stories featuring non-Western children disproportionately emphasize cultural heritage, tradition, and family themes far more than those for Western children. Our findings highlight the role of sociocultural bias in making creative AI use more equitable and diverse."
}
```

