### News

- `2024/5/11` We are working on a journal extension of CoRA where the eyeball position and radius are **automatically solved** from the data instead of manually set as in the CVPR'24 version; this part of code is now released! Stay tuned for the journal version paper.
- `2024/5/11` We have released the scripts and instructions to run on custom data!
- `2024/3/3` We have released the full code to run on our preprocessed dataset, see [Run.md](docs/Run.md) for more details.

# _CoRA_: _Co_-located *R*elightable *A*vatar

<img src="misc/teaser.gif" width="100%" >

This is a PyTorch implementation of the following paper:

**High-Quality Facial Geometry and Appearance Capture at Home with Automatic Eyeball Estimation**, CVPR 2024.

Yuxuan Han, Junfeng Lyu, and Feng Xu

[Project Page](https://yxuhan.github.io/CoRA/index.html) | [Video](https://www.youtube.com/watch?v=eqkTmNvlbgc) | [Paper](https://arxiv.org/abs/2312.03442)

**Abstract**: _Facial geometry and appearance capture have demonstrated tremendous success in 3D scanning real humans in studios. Recent works propose to democratize this technique while keeping the results high quality. However, they are still inconvenient for daily usage. In addition, they focus on an easier problem of only capturing facial skin. This paper proposes a novel method for high-quality face capture, featuring an easy-to-use system and the capability to model the complete face with skin, mouth interior, hair, and eyes. We reconstruct facial geometry and appearance from a single co-located smartphone flashlight sequence captured in a dim room where the flashlight is the dominant light source (e.g. rooms with curtains or at night). To model the complete face, we propose a novel hybrid representation to effectively model both eyes and other facial regions, along with novel techniques to learn it from images. We apply a combined lighting model to compactly represent real illuminations and exploit a morphable face albedo model as a reflectance prior to disentangle diffuse and specular. Experiments show that our method can capture high-quality 3D relightable scans._

## Document

To use our codebase to create your own 3D relightable avatar, we provide the following documents:

1. [Env.md](docs/Env.md) for code environment setup.
   - If you just want to quickly run the code on our released dataset, now you can directly goto [Run.md](docs/Run.md).
1. [Capture.md](docs/Capture.md) for instructions to capture video under our setup, i.e. co-located video in a dim room where the smartphone flashlight is the dominant light source.
1. [Preprocess.md](docs/Preprocess.md) for video preprocessing.
1. [Run.md](docs/Run.md) for scripts to train our method on the preprocessed dataset to reconstruct relightable avatar.

We also plan to create a video toturial to help users to create their own relightable avatar using our codebase. Stay tuned.

## Contact

If you have any questions, please contact Yuxuan Han (hanyx22@mails.tsinghua.edu.cn).

## License and Citation

This repository can <b>only be used for personal/research/non-commercial purposes</b>.
Please cite the following paper if it helps your research:

    @inproceedings{han2024cora,
        author = {Han, Yuxuan and Lyu, Junfeng and Xu, Feng},
        title = {High-Quality Facial Geometry and Appearance Capture at Home with Automatic Eyeball Estimation},
        journal={CVPR},
        year={2024}
    }

## Acknowledgments

- I would like to express my sincere gratitude to my lecturer,
  Prof. Owusu Agyemang, for their invaluable guidance, in-
  sightful feedback, and continuous support throughout this
  project. Their encouragement and expertise played a cru-
  cial role in the successful completion of this work.
  I am also deeply thankful to Mr. Dankla Luke for their un-
  wavering support, inspiration, and meaningful contributions
  during the development of this work. Their presence made
  this journey a memorable and fulfilling experience.
- The code is built on a bunch of wonderful projects, including: [Nerfacc](https://github.com/nerfstudio-project/nerfacc), [tinycudann](https://github.com/NVlabs/tiny-cuda-nn), [facer](https://github.com/FacePerceiver/facer), [metrical-tracker](https://github.com/Zielon/metrical-tracker), [AlbedoMM](https://github.com/waps101/AlbedoMM), [RobustVideoMatting](https://github.com/PeterL1n/RobustVideoMatting), and [WildLight](https://github.com/za-cheng/WildLight).
- Thanks [SoulShell](http://soulshell.cn/) for providing their Light Stage to help us conduct comparison experiments.
- Thanks [Jingwang Ling](https://gerwang.github.io/) and [Zhibo Wang](https://sireer.github.io/) for helpful discussions.
