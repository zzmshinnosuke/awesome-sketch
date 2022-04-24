# Related Works for Sketch learning

## Code and Framework
[sketch-rnn](https://github.com/magenta/magenta/tree/master/magenta/models/sketch_rnn)  
[torchsketch](https://github.com/PengBoXiangShang/torchsketch)  
[Awesome-Sketch-Synthesis](https://github.com/MarkMoHR/Awesome-Sketch-Synthesis)

## Table of Contents
* [Sketch Datasets](#Datasets)
* [Sketch Papers by Year](https://github.com/zzmshinnosuke/awesome-sketch/blob/master/paper-by-year.md)
* [Sketch Papers by content](https://github.com/zzmshinnosuke/awesome-sketch/blob/master/paper-by-content.md)

## Datasets
<table>
    <tr>
        <td><strong>Type</strong></td>
        <td><strong>Dataset</strong></td>
        <td><strong>Vector</strong></td>
        <td><strong>Paired</strong></td>
        <td><strong>Paper</strong></td> 
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
        <td rowspan="6"><strong>Object</strong></td>
        <td><a href="http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/">TU-Berlin</a></td>
        <td>&check;(svg)</td>
        <td>&cross;</td>
        <td><a href="http://cybertron.cg.tu-berlin.de/eitz/pdf/2012_siggraph_classifysketch.pdf">SIGGRAPH 2012</a></td>
        <td>250 categories; 80 sketch/cat; 20k sketches</td>
        <td>first large-scale scene sketch</td>
    </tr>
    <tr>
        <td><a href="http://sketchy.eye.gatech.edu/">Sketchy</a></td>
        <td>&check;(svg)</td>
        <td>&check;</td>
        <td><a href="https://dl.acm.org/doi/pdf/10.1145/2897824.2925954">SIGGRAPH 2016</a></td>
        <td>125 categories; 75471 sketches; 12500 images</td>
        <td>Each image corresponds to five sketches</td>
    </tr>
    <tr>
        <td><a href="https://quickdraw.withgoogle.com/data">Quickdraw</a></td>
        <td>&check;(5-tuple)</td>
        <td>&cross;</td>
        <td><a href="https://openreview.net/forum?id=Hy6GHpkCW">ICLR 2018</a></td>
        <td>345 categories; 10k/cat; 50M sketches</td>
        <td>huge amounts</td>
    </tr>
    <tr>
        <td><a href="http://sketchx.eecs.qmul.ac.uk/downloads/">QMUL-Shoe-V2</a></td>
        <td>&cross;(mat)</td>
        <td>&cross;</td>
        <td><a href="https://openaccess.thecvf.com/content_cvpr_2016/papers/Yu_Sketch_Me_That_CVPR_2016_paper.pdf">CVPR 2016</a></td>
        <td>2 categries; 700 sketches</td>
        <td>chair and shoe</td>
    </tr>
    <tr>
        <td><a href="https://github.com/HaohanWang/ImageNet-Sketch">ImageNet-Sketch</a></td>
        <td>&cross;</td>
        <td>&cross;</td>
        <td><a href="https://proceedings.neurips.cc/paper/2019/file/3eefceb8087e964f89c2d59e8a249915-Paper.pdf">NIPS 2019</a></td>
        <td>50000 sketches(image); 1000 ImageNet categories</td>
        <td>object, shadow</td>
    </tr>
    <tr>
        <td><a href="https://github.com/zachzeyuwang/tracing-vs-freehand">Tracing-Freehand</a></td>
        <td>&check;</td>
        <td>&check;</td>
        <td><a href="https://graphics.cs.yale.edu/sites/default/files/tracing-vs-freehand_0.pdf">SIGGRAPH 2021</a></td>
        <td>1210 Tracing；288 Freehand</td>
        <td></td>
    </tr>
    <tr>
        <td rowspan="6"><strong>Scene</strong></td>
        <td><a href="https://github.com/SketchyScene/SketchyScene">SketchyScene</a></td>
        <td>&cross;(mat)</td>
        <td>&check;</td>
        <td><a href="https://arxiv.org/abs/1808.02473">ECCV 2018</a></td>
        <td>train:5617; test:1113; val:535</td>
        <td>scene sketch</td>
    </tr>
    <tr>
        <td><a href="https://github.com/sysu-imsl/SketchyCOCO">SketchyCOCO</a></td>
        <td>&cross;(mat)</td>
        <td>&check;</td>
        <td><a href="https://openaccess.thecvf.com/content_CVPR_2020/papers/Gao_SketchyCOCO_Image_Generation_From_Freehand_Scene_Sketches_CVPR_2020_paper.pdf">CVPR 2020</a></td>
        <td>train:11265 ; test:2816</td>
        <td>scene sketches corresponding to real images</td>
    </tr>
    <tr>
        <td><a href="http://projects.csail.mit.edu/cmplaces/">CMPlaces</a></td>
        <td>&cross;</td>
        <td>&check;</td>
        <td><a href="http://cmplaces.csail.mit.edu/content/paper.pdf">TPAMI 2018</a></td>
        <td>train:6644; test:2050</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="https://github.com/EternalConfession/Context-Based-Sketch-Classification-Data">Context-Skecth</a></td>
        <td>&cross;</td>
        <td>&check;</td>
        <td><a href="http://sweb.cityu.edu.hk/hongbofu/doc/context_based_sketch_classification_Expressive2018.pdf">Expressive 2018</a></td>
        <td>354 sketches</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="http://www.cs.cmu.edu/~mengtial/proj/sketch/">Photo-Sketching</a></td>
        <td>&check;(svg)</td>
        <td>&check;</td>
        <td><a href="https://arxiv.org/abs/1901.00542">WACV 2019</a></td>
        <td>5000 sketches；1000 images</td>
        <td>scene sketch。trace</td>
    </tr>
    <tr>
        <td>SFSD</a></td>
        <td>&check;</td>
        <td>&check;</td>
        <td></td>
        <td>12000 sketches</td>
        <td>freehand scene sketch</td>
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



