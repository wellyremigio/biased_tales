# Biased Tales 

Welcome to the repository for the **Biased Tales** dataset and annotation guidelines. The dataset is also available on Hugging Face:  

👉 [Donya/biased_tales](https://huggingface.co/datasets/Donya/biased_tales)

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
@article{rooein2025biased,
  title={Biased Tales: Cultural and Topic Bias in Generating Children's Stories},
  author={Rooein, Donya and Zouhar, Vil{\'e}m and Nozza, Debora and Hovy, Dirk},
  journal={arXiv preprint arXiv:2509.07908},
  year={2025}
}
```

