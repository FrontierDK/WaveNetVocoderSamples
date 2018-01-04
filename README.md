# WaveNet Vocoder Samples

![](figure/overview.bmp)

## Audio samples

Audio examples are in `wav/<speaker_name>/<method>/arctic_<utt_id>.wav`

- `<speaker_id>`: the name of speaker in CMU Arctic database
  - `bdl`,` rms`: male speaker
  - `slt`, `clb`: female speaker
- `<method>` : the name of method
  - `raw`: target speech
  - `straight`: the conventional vocoder with F0, straight-melcep, aperiodicity
  - `sd`: the speaker-dependent WaveNet vocoder 
  - `sc_close`: the WaveNet vocoder with speaker-code trained using utterances of all of the speakers
  - `si_close`: the WaveNet vocoder trained using utterances of all of the speakers
  - `si_open`: the WaveNet vocoder trained using utterances of all of the speakers except for evaluation speakers

## Subjective Evaluation Result

- `#evaluation speakers=4` and `#evaluation utts per speaker=40`
- `#subjects=9` and `#evaluation utts per subject=120`

![mos](./figure/mos.bmp)

## Reference

```
@article{hayashi2018sp,
  title={複数話者WaveNetボコーダに関する調査}.
  author={林知樹 and 小林和弘 and 玉森聡 and 武田一哉 and 戸田智基},
  journal={電子情報通信学会技術研究報告},
  year={2018}
}
@article{hayashi2017multi,
  title={An Investigation of Multi-Speaker Training for WaveNet Vocoder},
  author={Hayashi, Tomoki and Tamamori, Akira and Kobayashi, Kazuhiro and Takeda, Kazuya and Toda, Tomoki},
  journal={Proc. ASRU 2017},
  year={2017}
}
```



