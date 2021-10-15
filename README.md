# Related Works for Sketch learning

## Code and Framework
[sketch-rnn](https://github.com/magenta/magenta/tree/master/magenta/models/sketch_rnn)  
[torchsketch](https://github.com/PengBoXiangShang/torchsketch)


## Table of Contents
* [Sketch Dataset](#Dataset)
* [Sketch Semantic Segmentation](#Sketch-Semantic-Segmentation)
* [Sketch-Based Image Retrival](#SBIR)


## Datasets
<table>
    <tr>
        <td><strong>Type</strong></td>
        <td><strong>Dataset</strong></td>
        <td><strong>Vector</strong></td>
        <td><strong>Paired</strong></td>
        <td><strong>Source</strong></td> 
        <td><strong>Scale</strong></td> 
        <td><strong>Remark</strong></td> 
    </tr>
    <tr>
        <td rowspan="3"><strong>Character</strong></td>
        <td><a href="https://github.com/brendenlake/omniglot/">Omniglot</a></td>
        <td>&check;</td>
        <td>&cross;</td>
        <td></td>
        <td></td>
        <td>Alphabets characters</td>
    </tr>
    <tr>
        <td><a href="http://kanjivg.tagaini.net/">KanjiVG</a></td>
        <td>&check;</td>
        <td>&cross;</td>
        <td></td>
        <td></td>
        <td>Chinese characters</td>
    </tr>
    <tr>
        <td><a href="https://github.com/rois-codh/kmnist">Kuzushiji</a></td>
        <td>&cross;</td>
        <td>&cross;</td>
        <td></td>
        <td></td>
        <td>Japanese characters</td>
    </tr>
    <tr>
        <td rowspan="4"><strong>Instance</strong></td>
        <td><a href="http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/">TU-Berlin</a></td>
        <td>&check;(svg)</td>
        <td>&cross;</td>
        <td>SIGGRAPH 2012</td>
        <td>250 categories; 80 sketch/cat; 20k sketches</td>
        <td>第一个大规模的草图数据集、比较形象</td>
    </tr>
    <tr>
        <td><a href="http://sketchy.eye.gatech.edu/">Sketchy</a></td>
        <td>&check;(svg)</td>
        <td>&check;</td>
        <td>SIGGRAPH 2016</td>
        <td>125 categories; 75471 sketches; 12500 images</td>
        <td>草图和图片一一对应</td>
    </tr>
    <tr>
        <td><a href="https://openreview.net/forum?id=Hy6GHpkCW">Quickdraw</a></td>
        <td>&check;(5-tuple)</td>
        <td>&cross;</td>
        <td>ICLR 2018</td>
        <td>345 categories; 10k/cat</td>
        <td>数据量大、抽象性高、噪音多</td>
    </tr>
    <tr>
        <td><a href="https://www.eecs.qmul.ac.uk/~qian/Project_cvpr16.html">QMUL-Shoe-V2</a></td>
        <td>&cross;(mat)</td>
        <td>&cross;</td>
        <td>CVPR 2018</td>
        <td>2 categries; 700 sketches</td>
        <td>包含两类物体椅子和鞋，跟图片对应的准确率更高</td>
    </tr>
    <tr>
        <td rowspan="6"><strong>Scene</strong></td>
        <td><a href="https://arxiv.org/abs/1808.02473">SketchyScene</a></td>
        <td>&cross;(mat)</td>
        <td>&check;</td>
        <td>ECCV 2018</td>
        <td>train:5617; test:1113; val:535</td>
        <td>场景图、草图和图像对应、图片是动漫图片</td>
    </tr>
    <tr>
        <td><a href="https://openaccess.thecvf.com/content_CVPR_2020/papers/Gao_SketchyCOCO_Image_Generation_From_Freehand_Scene_Sketches_CVPR_2020_paper.pdf">SketchyCOCO</a></td>
        <td>&cross;(mat)</td>
        <td>&check;</td>
        <td>CVPR 2020</td>
        <td>train:11265 ; test:2816</td>
        <td>与图像对应的场景草图数据集</td>
    </tr>
    <tr>
        <td><a href="http://projects.csail.mit.edu/cmplaces/">CMPlaces</a></td>
        <td>&cross;</td>
        <td>&check;</td>
        <td>TPAMI 2018</td>
        <td>train:6644; test:2050</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="http://sweb.cityu.edu.hk/hongbofu/doc/context_based_sketch_classification_Expressive2018.pdf">Context-Skecth</a></td>
        <td>&cross;</td>
        <td>&check;</td>
        <td>Expressive 2018</td>
        <td>354 sketches</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="http://www.cs.cmu.edu/~mengtial/proj/sketch/">Photo-Sketching</a></td>
        <td>&check;(svg)</td>
        <td>&check;</td>
        <td>WACV 2019</td>
        <td>5000 sketches；1000 images</td>
        <td>场景草图，但是没有单个物体的标注。trace</td>
    </tr>
    <tr>
        <td><a href="">ours</a></td>
        <td>&check;</td>
        <td>&check;</td>
        <td></td>
        <td></td>
        <td>sketch-text-image对应、同时包含单物体或多物体、包含普通和专业人士绘制</td>
    </tr>
    <tr>
        <td rowspan="1"><strong>CAD</strong></td>
        <td><a href=""></a></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
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


