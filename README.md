# A-Survey-of-Pluralistic-Alignment

- Reading list

  - (2023/03/30) [Whose Opinions Do Language Models Reflect?](https://arxiv.org/pdf/2303.17548)
  	- motivation: discussion
  	- focus: distributional pluralism
  	- contribution: OpinionQA dataset
  - (2023/05/24) [Aligning Language Models to User Opinions](https://arxiv.org/pdf/2305.14929)
  - (2023/10/17) [Group Preference Optimization: Few-Shot Alignment of Large Language Models](https://arxiv.org/pdf/2310.11523)
  - (2024/02/14) [MaxMin-RLHF: Towards Equitable Alignment of Large Language Models with Diverse Human Preferences](https://arxiv.org/pdf/2402.08925)
  	- motivation: discussion
  	- feature: theoretical proof
  - (2024/04/02) [Value Kaleidoscope: Engaging AI with Pluralistic Human Values, Rights, and Duties](https://arxiv.org/pdf/2309.00779)
  - (2024/04/24) [The PRISM Alignment Project: What Participatory, Representative and Individualised Human Feedback Reveals About the Subjective and Multicultural Alignment of Large Language Models](https://arxiv.org/pdf/2404.16019)
  	- feature: preferences (on LM-generated content) from global respondents on diverse (potentially controversial) topics
  	- limitation: data collected from real human respondents? (evaluation issue)
  - (2024/05/23) [Direct Preference Optimization With Unobserved Preference Heterogeneity](https://arxiv.org/pdf/2405.15065)
  	- feature: reward modeling for heterogeneous preferences
  - (2024/05/27) [RLHF from Heterogeneous Feedback via Personalization and Preference Aggregation](https://arxiv.org/pdf/2405.00254)
  	- feature: preference aggregation via human user clustering
  - (2024/06/12) [PAL: Pluralistic Alignment Framework for Learning from Heterogeneous Preferences](https://arxiv.org/pdf/2406.08469)WW

  - (2024/07/24) [PERSONA: A Reproducible Testbed for Pluralistic Alignment](https://arxiv.org/pdf/2407.17387)
  	- feature: synthetic personas (can be applied to role-playing LMs)
  - (2024/08/20) [A Roadmap to Pluralistic Alignment](https://arxiv.org/pdf/2402.05070)
  	- motivation: discussion, survey
  - (2024/10/11) [Modular Pluralism: Pluralistic Alignment via Multi-LLM Collaboration](https://arxiv.org/pdf/2406.15951)

- Methodologies mentioned

	- RLHF
	- DPO
	- EM-DPO、MinMax-DPO
		- Plackett-Luce model
		- Bradley-Terry-Luce model
	- Inverse RL → (Multiple) Reward Modeling
	- [GPO (Group Preference Optimization)](https://arxiv.org/pdf/2310.11523)

- Testbeds mentioned

  - [OpinionQA dataset](https://arxiv.org/pdf/2303.17548)
    - multiple-choice questions
    - 22 US demographic groups
  - [GlobalOpinionQA dataset](https://arxiv.org/pdf/2306.16388)
    - multiple-choice questions
    - 14 countries
  - [MoralChoice](Evaluating the Moral Beliefs Encoded in LLMs)
    - 687 low-ambiguous scenarios & 680 high-ambiguous scenarios
    - associated with uncertainty
  - [ValuePrism](https://arxiv.org/pdf/2309.00779)
    - 218k values, rights and duties ~ 31k human-written situations
  - the Pew Global Attitudes Survey
  - the World Values Survey
  - [PRISM dataset](https://arxiv.org/pdf/2404.16019)
  - contextual bandit experiment

- Metrics mentioned
	- Alignment Score: $\mathcal A(P_1, P_2; Q) = \frac{1}{|Q|} \sum_{q \in Q} Sim(P_1(q), P_2(q))$
	- Cohen’s kappa coefficient

- Definitions
	- Demographics: region, sex, age, education, race, citizen, marital status, and income.
	- Ideology: conservative, liberal, …

- Related topics
	- preference learning/preference aggregation
	- social simulation
	- social choice theory
	- representation learning