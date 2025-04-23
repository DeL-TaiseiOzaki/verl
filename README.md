<div align="center">
 👋 みなさん、こんにちは！ 
    <br>
    verl は <b>ByteDance Seed チーム</b>によって開始され、verl コミュニティによって維持されている強化学習トレーニングライブラリです。
</div>
<div align="center">
  以下のチャンネルを通じて Bytedance Seed についてより詳しく知ることができます👇
  <br>
  <a href="https://team.doubao.com/">
    <img src="https://img.shields.io/badge/Website-%231e37ff?style=for-the-badge&logo=bytedance&logoColor=white"></a>
  <a href="https://github.com/user-attachments/assets/469535a8-42f2-4797-acdf-4f7a1d4a0c3e">
    <img src="https://img.shields.io/badge/WeChat-07C160?style=for-the-badge&logo=wechat&logoColor=white"></a>
 <a href="https://www.xiaohongshu.com/user/profile/668e7e15000000000303157d?xsec_token=ABl2-aqekpytY6A8TuxjrwnZskU-6BsMRE_ufQQaSAvjc%3D&xsec_source=pc_search">
    <img src="https://img.shields.io/badge/Xiaohongshu-%23FF2442?style=for-the-badge&logo=xiaohongshu&logoColor=white"></a>
  <a href="https://www.zhihu.com/org/dou-bao-da-mo-xing-tuan-dui/">
    <img src="https://img.shields.io/badge/zhihu-%230084FF?style=for-the-badge&logo=zhihu&logoColor=white"></a>

</div>

![seed logo](https://github.com/user-attachments/assets/c42e675e-497c-4508-8bb9-093ad4d1f216)

<h1 style="text-align: center;">verl: Volcano Engine Reinforcement Learning for LLMs</h1>

<div align="center">

  [![GitHub Repo stars](https://img.shields.io/github/stars/volcengine/verl)](https://github.com/volcengine/verl/stargazers)
  ![GitHub forks](https://img.shields.io/github/forks/volcengine/verl)
  [![Twitter](https://img.shields.io/twitter/follow/verl_project)](https://twitter.com/verl_project)
  <a href="https://join.slack.com/t/verlgroup/shared_invite/zt-2w5p9o4c3-yy0x2Q56s_VlGLsJ93A6vA"><img src="https://img.shields.io/badge/Slack-verl-blueviolet?logo=slack&amp"></a>
  <a href="https://arxiv.org/pdf/2409.19256"><img src="https://img.shields.io/static/v1?label=EuroSys&message=Paper&color=red"></a>
  ![GitHub contributors](https://img.shields.io/github/contributors/volcengine/verl)
  [![Documentation](https://img.shields.io/badge/documentation-blue)](https://verl.readthedocs.io/en/latest/)
  <a href="https://raw.githubusercontent.com/eric-haibin-lin/verl-community/refs/heads/main/WeChat.JPG"><img src="https://img.shields.io/badge/微信-green?logo=wechat&amp"></a>

</div>



verl は、大規模言語モデル（LLM）向けの柔軟で効率的、かつ本番環境で使用可能な強化学習トレーニングライブラリです。

verl は **[HybridFlow: A Flexible and Efficient RLHF Framework](https://arxiv.org/abs/2409.19256v2)** 論文のオープンソース版です。

verl は柔軟で使いやすい以下の特徴を持っています：

- **多様な強化学習アルゴリズムの簡単な拡張**: ハイブリッドコントローラープログラミングモデルにより、複雑なポストトレーニングデータフローを柔軟に表現し効率的に実行できます。GRPO、PPOなどの強化学習データフローを数行のコードで構築できます。

- **モジュラーAPIによる既存のLLMインフラとのシームレスな統合**: 計算とデータの依存関係を分離し、FSDP、Megatron-LM、vLLM、SGLangなどの既存のLLMフレームワークとのシームレスな統合を可能にします。

- **柔軟なデバイスマッピング**: 効率的なリソース利用と異なるクラスターサイズでのスケーラビリティのために、異なるGPUセットにモデルを配置する様々な方法をサポートします。

- 人気のHuggingFaceモデルとの統合が容易


verl は高速です：

- **最先端のスループット**: 最先端のLLMトレーニングと推論エンジンの統合、および最先端の強化学習スループット。

- **3D-HybridEngineによる効率的なアクターモデルの再シャーディング**: トレーニングと生成フェーズの間の遷移中にメモリの冗長性を排除し、通信オーバーヘッドを大幅に削減します。

</p>

## ニュース
- [2025/05] verl は [GOSIM x PyTorch Day 2025](https://paris2025.gosim.org/) で発表されます。パリでお会いしましょう！
- [2025/04] [ICLR 2025 Expo](https://iclr.cc/virtual/2025/calendar?filter_events=Expo+Talk+Panel&filter_rooms=)、[SCI-FM ワークショップ](https://open-foundation-model.github.io/)、[LMSys アフターパーティ](https://lu.ma/d23nyynm)にて、最新のポストトレーニング技術とverlのプログラミングガイドについてチュートリアルを行います。シンガポールでお会いしましょう！
- [2025/04] [Seed-Thinking-v1.5](https://github.com/ByteDance-Seed/Seed-Thinking-v1.5/blob/main/seed-thinking-v1.5.pdf) 技術レポートがリリースされました！verl でトレーニングされた Seed-Thinking-v1.5 は AIME 2024 で 86.7、Codeforces で 55.0、GPQA で 77.3 を達成し、STEMとコーディングにおける優れた推論能力を示しています。推論タスクだけでなく、多様な領域にわたる顕著な一般化能力も示しています。
- [2025/04] 推論モデル向けの最新RL手法である [VAPO](https://arxiv.org/pdf/2504.05118)（value-based augmented PPO）のオープンソースレシピに取り組んでいます。Qwen-32B-baseモデルからトレーニングされたVAPOは、AIME 2024で60.4を達成し、DeepSeek-zero-32BとDAPO-32Bを上回っています。
- [2025/03] verl v0.3.0.post1 がリリースされました！詳細は[リリースノート](https://github.com/volcengine/verl/releases/)をご覧ください。
- [2025/03] [DAPO](https://dapo-sia.github.io/) は、Qwen2.5-32B事前学習モデルをベースにAIME 2024で50ポイントを達成した最先端のRLアルゴリズムで、DeepSeekのGRPO（DeepSeek-R1-Zero-Qwen-32B）による以前の最高記録を上回っています。DAPOのトレーニングはverlによって完全に実現され、再現コードは `recipe/dapo` で利用可能です。
<details><summary> もっと見る... </summary>
<ul>
  <li>[2025/03] [vLLM 北京ミートアップ](https://mp.weixin.qq.com/s/n77GibL2corAtQHtVEAzfg)でverlのプログラミングモデルを紹介し、3月中旬にサニーベールで開催された[SGLang-LMSYS Org ミートアップ](https://lu.ma/ntjrr7ig)で[verl紹介と更新情報](https://github.com/eric-haibin-lin/verl-community/blob/main/slides/verl-lmsys-meetup.pdf)を発表しました。</li>
  <li>[2025/02] verl v0.2.0.post2 がリリースされました！</li>
  <li>[2025/01] [Doubao-1.5-pro](https://team.doubao.com/zh/special/doubao_1_5_pro) がLLMとVLMで最先端レベルのパフォーマンスで公開されました。RLスケーリングプレビューモデルはverlを使用してトレーニングされ、数学ベンチマーク（AIMEでpass@1が70.0）でOpenAI O1レベルのパフォーマンスに到達しています。</li>
  <li>[2025/03] EuroSys 2025でverl(HybridFlow)を発表します。ロッテルダムでお会いしましょう！</li>
  <li>[2025/02] <a href="https://lu.ma/ji7atxux">Bytedance/NVIDIA/Anyscale Ray ミートアップ</a>でverlを発表しました。サンノゼでお会いしましょう！</li>
  <li>[2024/12] Ray Forward 2024でverlが発表されました。スライドは<a href="https://github.com/eric-haibin-lin/verl-community/blob/main/slides/Ray_Forward_2024_%E5%B7%AB%E9%94%A1%E6%96%8C.pdf">こちら</a>でご覧いただけます。</li>
  <li>[2024/10] Ray Summitでverlが発表されました。<a href="https://www.youtube.com/watch?v=MrhMcXkXvJU&list=PLzTswPQNepXntmT8jr9WaNfqQ60QwW7-U&index=37">Youtubeビデオ</a>でご覧いただけます。</li>
  <li>[2024/12] チームはNeurIPS 2024で<a href="https://neurips.cc/Expo/Conferences/2024/workshop/100677">Post-training LLMs: From Algorithms to Infrastructure</a>を発表しました。<a href="https://github.com/eric-haibin-lin/verl-data/tree/neurips">スライド</a>と<a href="https://neurips.cc/Expo/Conferences/2024/workshop/100677">ビデオ</a>が利用可能です。</li>
  <li>[2024/08] HybridFlow (verl) がEuroSys 2025に採択されました。</li>
</ul>   
</details>

## 主な機能

- トレーニングに**FSDP**と**Megatron-LM**を使用。
- ロールアウト生成に**vLLM**、**SGLang**、**HF Transformers**を使用。
- Hugging Face TransformersとModelscope Hubとの互換性：Qwen-2.5、Llama3.1、Gemma2、DeepSeek-LLMなど
- 教師付き微調整。
- [PPO](examples/ppo_trainer/)、[GRPO](examples/grpo_trainer/)、[ReMax](examples/remax_trainer/)、[REINFORCE++](https://verl.readthedocs.io/en/latest/examples/config.html#algorithm)、[RLOO](examples/rloo_trainer/)、[PRIME](recipe/prime/)、[DAPO](recipe/dapo/)、[DrGRPO](recipe/drgrpo)などの強化学習。
  - モデルベースの報酬と関数ベースの報酬（検証可能な報酬）をサポート
  - ビジョン言語モデル（VLM）と[マルチモーダルRL](examples/grpo_trainer/run_qwen2_5_vl-7b.sh)をサポート
- Flash attention 2、[シーケンスパッキング](examples/ppo_trainer/run_qwen2-7b_seq_balance.sh)、DeepSpeed Ulyssesによる[シーケンス並列処理](examples/ppo_trainer/run_deepseek7b_llm_sp2.sh)、[LoRA](examples/sft/gsm8k/run_qwen_05_peft.sh)、[Ligerカーネル](examples/sft/gsm8k/run_qwen_05_sp2_liger.sh)をサポート。
- 70Bモデルと数百のGPUまでスケール。
- wandb、swanlab、mlflow、tensorboardによる実験追跡。

## 今後の機能
- ロードマップ https://github.com/volcengine/verl/issues/710 
- Megatron v0.11によるDeepSeek 671bの最適化 https://github.com/volcengine/verl/issues/708 
- マルチターンロールアウトの最適化 https://github.com/volcengine/verl/pull/1037 https://github.com/volcengine/verl/pull/1138
- 環境インタラクション https://github.com/volcengine/verl/issues/1172 

## はじめに

<a href="https://verl.readthedocs.io/en/latest/index.html"><b>ドキュメント</b></a>

**クイックスタート:**
- [インストール方法](https://verl.readthedocs.io/en/latest/start/install.html)
- [クイックスタート](https://verl.readthedocs.io/en/latest/start/quickstart.html)
- [プログラミングガイド](https://verl.readthedocs.io/en/latest/hybrid_flow.html)

**PPOの例をステップバイステップで実行する:**
- データと報酬の準備
  - [ポストトレーニング用のデータ準備](https://verl.readthedocs.io/en/latest/preparation/prepare_data.html)
  - [データセット用の報酬関数の実装](https://verl.readthedocs.io/en/latest/preparation/reward_function.html)
- PPOの例を理解する
  - [PPO例のアーキテクチャ](https://verl.readthedocs.io/en/latest/examples/ppo_code_architecture.html)
  - [設定の説明](https://verl.readthedocs.io/en/latest/examples/config.html)
  - [GSM8Kの例を実行する](https://verl.readthedocs.io/en/latest/examples/gsm8k_example.html)

**再現可能なアルゴリズムのベースライン:**
- [PPO、GRPO、ReMax](https://verl.readthedocs.io/en/latest/experiment/ppo.html)

**コード説明と高度な使用方法（拡張）:**
- PPOトレーナーとワーカー
  - [PPO Rayトレーナー](https://verl.readthedocs.io/en/latest/workers/ray_trainer.html)
  - [PyTorch FSDPバックエンド](https://verl.readthedocs.io/en/latest/workers/fsdp_workers.html)
  - [Megatron-LMバックエンド](https://verl.readthedocs.io/en/latest/index.html)
- 高度な使用方法と拡張
  - [Ray API設計チュートリアル](https://verl.readthedocs.io/en/latest/advance/placement.html)
  - [他のRL(HF)アルゴリズムへの拡張](https://verl.readthedocs.io/en/latest/advance/dpo_extension.html)
  - [FSDPバックエンドでのモデル追加](https://verl.readthedocs.io/en/latest/advance/fsdp_extension.html)
  - [Megatron-LMバックエンドでのモデル追加](https://verl.readthedocs.io/en/latest/advance/megatron_extension.html)
  - [別のGPUリソースを使用したデプロイメント](https://github.com/volcengine/verl/tree/main/examples/split_placement)

**コミュニティからのブログ**
- [使用verl进行GRPO分布式强化学习训练最佳实践](https://www.volcengine.com/docs/6459/1463942)
- [HybridFlow veRL 原文浅析](https://github.com/zhaochenyang20/Awesome-ML-SYS-Tutorial/blob/main/rlhf/verl/readme.md)
- [最高提升20倍吞吐量！豆包大模型团队发布全新 RLHF 框架，现已开源！](https://team.doubao.com/en/blog/%E6%9C%80%E9%AB%98%E6%8F%90%E5%8D%8720%E5%80%8D%E5%90%9E%E5%90%90%E9%87%8F-%E8%B1%86%E5%8C%85%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9B%A2%E9%98%9F%E5%8F%91%E5%B8%83%E5%85%A8%E6%96%B0-rlhf-%E6%A1%86%E6%9E%B6-%E7%8E%B0%E5%B7%B2%E5%BC%80%E6%BA%90)


## パフォーマンスチューニングガイド
オンポリシーRLアルゴリズムにとってパフォーマンスは不可欠です。パフォーマンスを最適化するための詳細な[パフォーマンスチューニングガイド](https://verl.readthedocs.io/en/latest/perf/perf_tuning.html)を用意しています。

## vLLM >= v0.8.2 へのアップグレード
verlはFSDPをトレーニングバックエンドとして使用する場合、vLLM>=0.8.2をサポートするようになりました。インストールガイドと詳細については[こちらのドキュメント](https://github.com/volcengine/verl/blob/main/docs/README_vllm0.8.md)を参照してください。OOMや予期せぬエラーを引き起こす可能性のあるバグを含むvllm 0.7.xは避けてください。

## 最新のSGLangを使用する
SGLangはverlで完全にサポートされており、SGLang RLグループはマルチターンエージェントRL、VLM RLHF、サーバーベースRL、部分的ロールアウトなどのユニークな機能の構築に積極的に取り組んでいます。インストールガイドと詳細については[こちらのドキュメント](https://verl.readthedocs.io/en/latest/workers/sglang_worker.html)を参照してください。

## [ハードウェア] AMD (ROCMm カーネル) のサポート
 verlは現在、トレーニングエンジンとしてFSDPをサポートし（Megatronのサポートは近日中）、推論エンジンとしてvLLMとSGLangの両方と統合しています。インストールガイドと詳細については[こちらのドキュメント](https://github.com/volcengine/verl/blob/main/docs/amd_tutorial/amd_build_dockerfile_page.rst)を参照してください。


## 引用と謝辞

このプロジェクトが役立つと感じた場合は、以下を引用してください：
- [HybridFlow: A Flexible and Efficient RLHF Framework](https://arxiv.org/abs/2409.19256v2)
- [A Framework for Training Large Language Models for Code Generation via Proximal Policy Optimization](https://i.cs.hku.hk/~cwu/papers/gmsheng-NL2Code24.pdf)

```bibtex
@article{sheng2024hybridflow,
  title   = {HybridFlow: A Flexible and Efficient RLHF Framework},
  author  = {Guangming Sheng and Chi Zhang and Zilingfeng Ye and Xibin Wu and Wang Zhang and Ru Zhang and Yanghua Peng and Haibin Lin and Chuan Wu},
  year    = {2024},
  journal = {arXiv preprint arXiv: 2409.19256}
}
```

verlはNemo-Aligner、Deepspeed-chat、OpenRLHFの設計にインスパイアされています。このプロジェクトはBytedance、Anyscale、LMSys.org、[Alibaba Qwenチーム](https://github.com/QwenLM/)、上海AI研究所、清華大学、UCバークレー、UCLA、UIUC、香港大学、ke.com、[All Hands AI](https://www.all-hands.dev/)、[ModelBest](http://modelbest.cn/)、[OpenPipe](https://openpipe.ai/)、JD AI研究所、マイクロソフトリサーチ、[StepFun](https://www.stepfun.com/)、Amazon、Linkedin、Meituan、[Camel-AI](https://www.camel-ai.org/)、[OpenManus](https://github.com/OpenManus)、Prime Intellect、NVIDIAリサーチ、[Baichuan](https://www.baichuan-ai.com/home)などによって採用・貢献されています。

## verlを使用した素晴らしい取り組み
- [TinyZero](https://github.com/Jiayi-Pan/TinyZero): 推論タスク向けの**DeepSeek R1 Zero**レシピの再現 ![GitHub Repo stars](https://img.shields.io/github/stars/Jiayi-Pan/TinyZero)
- [DAPO](https://dapo-sia.github.io/): DeepSeek-R1-zero-32Bを上回る完全オープンソースの最先端RLアルゴリズム ![GitHub Repo stars](https://img.shields.io/github/stars/volcengine/verl)
- [SkyThought](https://github.com/NovaSky-AI/SkyThought): NovaSky AIチームによるSky-T1-7BのRLトレーニング ![GitHub Repo stars](https://img.shields.io/github/stars/NovaSky-AI/SkyThought)
- [simpleRL-reason](https://github.com/hkust-nlp/simpleRL-reason): SimpleRL-Zoo: 野生のオープンベースモデルのためのゼロ強化学習の調査と制御 ![GitHub Repo stars](https://img.shields.io/github/stars/hkust-nlp/simpleRL-reason)
- [Easy-R1](https://github.com/hiyouga/EasyR1): **マルチモーダル**RLトレーニングフレームワーク ![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/EasyR1)
- [OpenManus-RL](https://github.com/OpenManus/OpenManus-RL): 複数のエージェント環境向けLLMエージェントRLチューニングフレームワーク ![GitHub Repo stars](https://img.shields.io/github/stars/OpenManus/OpenManus-RL)
- [deepscaler](https://github.com/agentica-project/rllm/tree/deepscaler): GRPOによる反復的コンテキストスケーリング ![GitHub Repo stars](https://img.shields.io/github/stars/agentica-project/deepscaler)
- [rllm](https://github.com/agentica-project/rllm): [verl-pipeline](https://github.com/agentica-project/verl-pipeline)による非同期RLトレーニング ![GitHub Repo stars](https://img.shields.io/github/stars/agentica-project/rllm)
- [PRIME](https://github.com/PRIME-RL/PRIME): 暗黙的報酬によるプロセス強化 ![GitHub Repo stars](https://img.shields.io/github/stars/PRIME-RL/PRIME)
- [RAGEN](https://github.com/ZihanWang314/ragen): 汎用推論**エージェント**トレーニングフレームワーク ![GitHub Repo stars](https://img.shields.io/github/stars/ZihanWang314/ragen)
- [Logic-RL](https://github.com/Unakar/Logic-RL): 2K Tiny Logic Puzzleデータセットを使用したDeepSeek R1 Zeroの再現 ![GitHub Repo stars](https://img.shields.io/github/stars/Unakar/Logic-RL)
- [Search-R1](https://github.com/PeterGriffinJin/Search-R1): 推論と**検索（ツールコール）**が交互に行われるLLMの強化学習 ![GitHub Repo stars](https://img.shields.io/github/stars/PeterGriffinJin/Search-R1)
- [ReSearch](https://github.com/Agent-RL/ReSearch): 強化学習によるLLMの**Re**asoningと**Search**の学習 ![GitHub Repo stars](https://img.shields.io/github/stars/Agent-RL/ReSearch)
- [DeepRetrieval](https://github.com/pat-jj/DeepRetrieval): **情報検索**のためのRLを通じたLLMによる**実際の検索エンジン**と**リトリーバー**のハッキング ![GitHub Repo stars](https://img.shields.io/github/stars/pat-jj/DeepRetrieval)
- [Code-R1](https://github.com/ganler/code-r1): 信頼性の高い報酬による**コード**用R1の再現 ![GitHub Repo stars](https://img.shields.io/github/stars/ganler/code-r1)
- [Skywork-OR1](https://github.com/SkyworkAI/Skywork-OR1): Skywork オープン推論シリーズ ![GitHub Repo stars](https://img.shields.io/github/stars/SkyworkAI/Skywork-OR1)
- [ToRL](https://github.com/GAIR-NLP/ToRL): ツール統合RLのスケーリング ![GitHub Repo stars](https://img.shields.io/github/stars/GAIR-NLP/ToRL)
- [cognitive-behaviors](https://github.com/kanishkg/cognitive-behaviors): 自己改善型推論を可能にする認知行動、または、高効率STaRの4つの習慣 ![GitHub Repo stars](https://img.shields.io/github/stars/kanishkg/cognitive-behaviors)
- [PURE](https://github.com/CJReinforce/PURE): **信用割り当て**は**プロセス報酬モデル**を使用した強化学習の成功の鍵 ![GitHub Repo stars](https://img.shields.io/github/stars/CJReinforce/PURE)
- [MetaSpatial](https://github.com/PzySeere/MetaSpatial): **メタバース**のための**VLM**における**3D空間推論**の強化 ![GitHub Repo stars](https://img.shields.io/github/stars/PzySeere/MetaSpatial)
- [DeepEnlighten](https://github.com/DolbyUUU/DeepEnlighten): **社会的推論**タスクでR1を再現し、主要な発見を分析 ![GitHub Repo stars](https://img.shields.io/github/stars/DolbyUUU/DeepEnlighten)
- [DeepResearcher](https://github.com/GAIR-NLP/DeepResearcher): 実世界環境での強化学習による深い研究のスケーリング ![GitHub Repo stars](