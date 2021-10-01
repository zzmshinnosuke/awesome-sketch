# Related Works for Sketch learning

## Code and Framework
[sketch-rnn](https://github.com/magenta/magenta/tree/master/magenta/models/sketch_rnn)  
[torchsketch](https://github.com/PengBoXiangShang/torchsketch)


## Table of Contents
* [Sketch Dataset](#Dataset)
* [Sketch Semantic Segmentation](#Sketch-Semantic-Segmentation)
* [Sketch-Based Image Retrival](#SBIR)


## Dataset
<table>
    <tr>
        <td> </td>
        <td><strong>Dataset</strong></td>
        <td><strong>Vector</strong></td>
        <td><strong>Paired</strong></td>
        <td><strong>Source</strong></td> 
        <td><strong>Scale</strong></td> 
        <td><strong>Remark</strong></td> 
    </tr>
    <tr>
        <td rowspan="3"><strong>Characters</strong></td>
        <td>Omniglob</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>KanjiVG</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>Kuzushiji</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td rowspan="4"><strong>Instance</strong></td>
        <td>TU-Berlin</td>
        <td>&check;</td>
        <td>&cross;</td>
        <td>SIGGRAPH 2012</td>
        <td>250 category 80张/类 20k张</td>
        <td>专业人士绘制、比较形象</td>
    </tr>
    <tr>
        <td>Sketchy</td>
        <td>&check;</td>
        <td>&check;</td>
        <td>SIGGRAPH 2016</td>
        <td>125类 75471张</td>
        <td>草图和图片一一对应</td>
    </tr>
    <tr>
        <td>Quickdraw</td>
        <td>&check;</td>
        <td>&cross;</td>
        <td>ICLR 2018</td>
        <td>345类 10k/类</td>
        <td>数据量大、抽象性高、噪音多</td>
    </tr>
    <tr>
        <td>QMUL-Shoe-V2</td>
        <td>&cross;</td>
        <td>&cross;</td>
        <td>CVPR 2018</td>
        <td>345类 10k/类</td>
        <td>包含两类物体椅子和鞋，跟图片对应</td>
    </tr>
    <tr>
        <td rowspan="3"><strong>Scene</strong></td>
        <td>SketchyScene</td>
        <td>&check;</td>
        <td>&cross;</td>
        <td>SIGGRAPH 2012</td>
        <td>250 category 80张/类 20k张</td>
        <td>专业人士绘制、比较形象</td>
    </tr>
    <tr>
        <td>SketchyCoCo</td>
        <td>&check;</td>
        <td>&cross;</td>
        <td>ICLR 2018</td>
        <td>345类 10k/类</td>
        <td>数据量大、抽象性高、噪音多</td>
    </tr>
    <tr>
        <td>Quickdraw</td>
        <td>&check;</td>
        <td>&cross;</td>
        <td>ICLR 2018</td>
        <td>345类 10k/类</td>
        <td>数据量大、抽象性高、噪音多</td>
    </tr>
</table>

## Sketch-Semantic-Segmentation
- [SketchGNN: Semantic Sketch Segmentation with Graph Neural Networks](https://dl.acm.org/doi/pdf/10.1145/3450284), TOG, 2021

- [Instance GNN: A Learning Framework for Joint Symbol Segmentation and Recognition in Online Handwritten Diagrams](http://www.nlpr.ia.ac.cn/databases/CASIA-OHFC/flowchart_recognition_TMM_2021-2nd%20submission.pdf)  , Multimedia, 2021, 
[dataset](http://www.nlpr.ia.ac.cn/databases/CASIA-OHFC/)

- [FloorPlanCAD: A Large-Scale CAD Drawing Dataset for Panoptic Symbol Spotting](https://arxiv.org/pdf/2105.07147.pdf), arXiv, 2021

- [SketchSegNet+: An End-to-End Learning of RNN for Multi-Class Sketch Semantic Segmentation](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8766108), IEEE Access, 2019

- [Bitmap or Vector? A study on sketch representations for deep stroke segmentation](https://hal.inria.fr/hal-02922043/document), JFIJ, 2019

- [Table Detection and Cell Segmentation in Online Handwritten Documents with Graph Attention Networks](https://dl.acm.org/doi/pdf/10.1145/3444685.3446295), Mutimedia Asia, 2021

- [Fast Sketch Segmentation and Labeling with Deep Learning](https://arxiv.org/pdf/1807.11847), CGA, 2018

- [Universal Sketch Perceptual Grouping](https://openaccess.thecvf.com/content_ECCV_2018/papers/Ke_LI_Universal_Sketch_Perceptual_ECCV_2018_paper.pdf), ECCV, 2018

- [Making Better Use of Edges via Perceptual Grouping](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Qi_Making_Better_Use_2015_CVPR_paper.pdf), CRPR, 2015

- [Data-driven Segmentation and Labeling of Freehand Sketches](https://dl.acm.org/doi/pdf/10.1145/2661229.2661280), TOG, 2014

- [Free Hand-Drawn Sketch Segmentation](https://link.springer.com/content/pdf/10.1007/978-3-642-33718-5_45.pdf), ECCV, 2012







## SBIR


