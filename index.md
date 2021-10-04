# K-Converter

## K-Converter: An unsupervised singing Voice Conversion System

### Abstract
<div style="text-align: justify"> Singing voice conversion (SVC) converts a singer's voice to another one's voice while preserving the linguistic content. Recently, some SVC systems rely on super-vised phonetic features extracted from pre-trained automatic speech recognition (ASR) models, increasing system complexity. Some end-to-end SVC systems use adver-sarial training, which causes instability during optimization. To address these issues, we present K-Converter, a simple system to disentangle the timbre, pitch, and content information without any manual supervision or adversarial training. First, low quefrencies of mel-frequency cepstral coefficients (MFCC), which remove the global excitation mainly, are used as input representation. And the pitch-shift augmentation is used for further disentangling the pitch. Second, an encoder network is carefully designed to construct an information bottleneck, which learns to break up the pitch and timbre information of the source. Third, the content consistency loss is introduced to keep the content consistent between encoder outputs of source utterances and reconstructed ones. Experimental results show that our proposed system performs well in both speech naturalness and timbre similarity, with better robustness to comparisons. </div>

<br>

### Model Architecture
<table border="0">
  <tbody>
    <tr>
      <td><img src="figs/kconverter.png" alt="Overall Architecture"></td>
    </tr>
  </tbody>
</table>

<br>


### Audio Samples

#### Target Singers
| Target   | Samples  |
|  ----  | ----  |
| Female| <audio id="audio" controls="" preload="none"><source id="wav" src="https://github.com/vcdemo-1/KConverter/blob/gh-pages/target_waves/f_biaobei_002_01.wav"></audio> |
| Male  | <audio id="audio" controls="" preload="none"><source id="wav" src="https://github.com/vcdemo-1/KConverter/blob/gh-pages/target_waves/m_biaobei_093_0001.wav"></audio> |

#### Source Singers
| Target   | Samples  |
|  ----  | ----  |
| F1| <audio id="audio" controls="" preload="none"><source id="wav" src="https://github.com/vcdemo-1/KConverter/blob/gh-pages/target_waves/f_biaobei_002_01.wav"></audio> |
| F2  | <audio id="audio" controls="" preload="none"><source id="wav" src="https://github.com/vcdemo-1/KConverter/blob/gh-pages/target_waves/m_biaobei_093_0001.wav"></audio> |
| M1  | <audio id="audio" controls="" preload="none"><source id="wav" src="https://github.com/vcdemo-1/KConverter/blob/gh-pages/target_waves/m_biaobei_093_0001.wav"></audio> |
| M2  | <audio id="audio" controls="" preload="none"><source id="wav" src="https://github.com/vcdemo-1/KConverter/blob/gh-pages/target_waves/m_biaobei_093_0001.wav"></audio> |
#### Comparison with Baseline Systems

| Systems|F1|F2|M1|M2|
|----|----|----|----|----|
|BASE1|||||
|BASE2|||||
|Ours|||||
#### Ablation 

