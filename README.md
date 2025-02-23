# Image-Matching-Paper-List
A personal list of papers and resources for image matching, pose estimation and some other 3D reconstruction tasks, including perspective images and panoramas (marked with :globe_with_meridians:).

---
- [Sparse matching (detector-based)](#sparse)
   - [Keypoints and descriptors](#keypoints-and-descriptors)
   - [Feature matching](#feature-matching)
- [Semi-dense matching (detector-free)](#semi-dense)
- [Dense matching](#dense)
- [Pose estimation and others](#pose-estimation-and-others)
- [Similar images disambiguate](#similar-images-disambiguate)
- [Datasets](#datasets)
- [Challenges and workshops](#challenges-and-workshops)
- [Resources](#resources)

Disambiguate Images of Similar Structures

---
## Sparse
### Keypoints and descriptors
   * ORB: An efficient alternative to SIFT or SURF [[ICCV 2011](http://www.evreninsirlari.net/dosyalar/145_s14_01.pdf)] [[]()]

   * :globe_with_meridians: SPHORB: A Fast and Robust Binary Feature on the Sphere [[IJCV 2015](http://cic.tju.edu.cn/faculty/lwan/paper/SPHORB/SPHORB.html)] [[SPHORB](https://github.com/tdsuper/SPHORB)]

   * Working hard to know your neighbor's margins: Local descriptor learning loss [[NeurIPS 2017](https://arxiv.org/pdf/1705.10872.pdf)] [[hardnet](https://github.com/DagnyT/hardnet)]

   * Repeatability Is Not Enough: Learning Discriminative Affine Regions via Discriminability [[ECCV 2018](https://arxiv.org/pdf/1711.06704.pdf)] [[affnet](https://github.com/ducha-aiki/affnet)]

   * Efficient adaptive non-maximal suppression algorithms for homogeneous spatial keypoint distribution [[Pattern Recognition Letters 2018](https://www.researchgate.net/publication/323388062_Efficient_adaptive_non-maximal_suppression_algorithms_for_homogeneous_spatial_keypoint_distribution)] [[ANMS-Codes](https://github.com/BAILOOL/ANMS-Codes)]

   * SuperPoint: Self-Supervised Interest Point Detection and Description [[CVPRW 2018](https://arxiv.org/pdf/1712.07629.pdf)] [[SuperPointPretrainedNetwork](https://github.com/magicleap/SuperPointPretrainedNetwork)]
   
   * Key.Net: Keypoint Detection by Handcrafted and Learned CNN Filters [[ICCV 2019](https://arxiv.org/pdf/1904.00889.pdf)] [[Key.Net-Pytorch](https://github.com/axelBarroso/Key.Net-Pytorch)]


   * D2-net: A trainable cnn for joint description and detection of local features [[CVPR 2019](https://openaccess.thecvf.com/content_CVPR_2019/papers/Dusmanu_D2-Net_A_Trainable_CNN_for_Joint_Description_and_Detection_of_CVPR_2019_paper.pdf)] [[d2-net](https://github.com/mihaidusmanu/d2-net)]

   * R2D2: Repeatable and Reliable Detector and Descriptor [[NeurIPS 2019](https://proceedings.neurips.cc/paper/2019/file/3198dfd0aef271d22f7bcddd6f12f5cb-Paper.pdf)] [[r2d2](https://github.com/naver/r2d2)]

   * ASLFeat: Learning Local Features of Accurate Shape and Localization [[CVPR 2020](https://arxiv.org/pdf/2003.10071.pdf)] [[ASLFeat](https://github.com/lzx551402/ASLFeat)]

   * DISK: Learning local features with policy gradient [[NeurIPS 2020](https://arxiv.org/pdf/2006.13566.pdf)] [[disk](https://github.com/cvlab-epfl/disk)]
   
   * Online Invariance Selection for Local Feature Descriptors [[ECCV 2020](https://arxiv.org/pdf/2007.08988.pdf)] [[LISRD](https://github.com/rpautrat/LISRD)]

   * Co-attention for conditioned image matching
    [[CVPR 2021](https://openaccess.thecvf.com/content/CVPR2021/papers/Wiles_Co-Attention_for_Conditioned_Image_Matching_CVPR_2021_paper.pdf)] [[coam](https://github.com/hyenal/coam)]
    
   * Rethinking Low-level Features for Interest Point Detection and Description [[ACCVC 2022](https://openaccess.thecvf.com/content/ACCV2022/papers/Wang_Rethinking_Low-level_Features_for_Interest_Point_Detection_and_Description_ACCV_2022_paper.pdf)] [[lanet](https://github.com/wangch-g/lanet)]   
   
   * ALIKE: Accurate and Lightweight Keypoint Detection and Descriptor Extraction [[TMM 2022](https://arxiv.org/pdf/2112.02906.pdf)] [[ALIKE](https://github.com/Shiaoming/ALIKE)]

   * Decoupling Makes Weakly Supervised Local Feature Better [[CVPR 2022](https://openaccess.thecvf.com/content/CVPR2022/papers/Li_Decoupling_Makes_Weakly_Supervised_Local_Feature_Better_CVPR_2022_paper.pdf)] [[PoSFeat](https://github.com/The-Learning-And-Vision-Atelier-LAVA/PoSFeat)]

   * Shared Coupling-bridge for Weakly Supervised Local Feature Learning [[arXiv 2022](https://arxiv.org/pdf/2212.07047.pdf)] [[SCFeat](https://github.com/sunjiayuanro/SCFeat)]

   * Self-Supervised Equivariant Learning for Oriented Keypoint Detection [[CVPR 2022](https://arxiv.org/pdf/2204.08613.pdf)] [[REKD](https://github.com/bluedream1121/REKD)]

   * Robust feature matching via progressive smoothness consensus [[ISPRS 2023](https://www.sciencedirect.com/science/article/abs/pii/S0924271623000229)] [[Robust-feature-matching-via-Progressive-Smoothness-Consensus](https://github.com/XiaYifan1999/Robust-feature-matching-via-Progressive-Smoothness-Consensus)]
  
  * SiLK: Simple Learned Keypoints [[ICCV 2023](https://arxiv.org/pdf/2304.06194v1.pdf)] [[silk](https://github.com/facebookresearch/silk)]
  
  * ALIKED: A Lighter Keypoint and Descriptor Extraction Network via Deformable Transformation [[IEEE Trans Instrum Meas 2023](https://arxiv.org/pdf/2304.03608.pdf)] [[ALIKED](https://github.com/Shiaoming/ALIKED)]

  * MTLDesc: Looking Wider to Describe Better [[AAAI 2022](https://arxiv.org/pdf/2203.07003.pdf)] [[mtldesc](https://github.com/vignywang/mtldesc)]

  * Attention Weighted Local Descriptors [[TPAMI 2023](https://ieeexplore.ieee.org/abstract/document/10105519/)] [[AWDesc](https://github.com/vignywang/AWDesc)]
  
  * FeatureBooster: Boosting Feature Descriptors with a Lightweight Neural Network [[CVPR 2023](https://arxiv.org/pdf/2211.15069.pdf)] [[FeatureBooster](https://github.com/SJTU-ViSYS/FeatureBooster)]

  * SFD2: Semantic-guided Feature Detection and Description [[arXiv 2023](https://arxiv.org/pdf/2304.14845.pdf)] [[sfd2](https://github.com/feixue94/sfd2)]

  * :globe_with_meridians: PanoPoint: Self-Supervised Feature Points Detection and Description for 360° Panorama [[CVPR 2023](https://openaccess.thecvf.com/content/CVPR2023W/OmniCV/papers/Zhang_PanoPoint_Self-Supervised_Feature_Points_Detection_and_Description_for_360deg_Panorama_CVPRW_2023_paper.pdf)] [[]()]

  * DeDoDe: Detect, Don't Describe -- Describe, Don't Detect for Local Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2308.08479.pdf)] [[DeDoDe](https://github.com/Parskatt/DeDoDe)]
    
  * S-TREK: Sequential Translation and Rotation Equivariant Keypoints for local feature extraction [[arXiv 2023](https://arxiv.org/pdf/2308.14598.pdf)] [[]()]

  * DarkFeat: Noise-Robust Feature Detector and Descriptor for Extremely Low-Light RAW Images [[AAAI 2023](https://ojs.aaai.org/index.php/AAAI/article/view/25161)] [[DarkFeat](https://github.com/THU-LYJ-Lab/DarkFeat)]

### Feature matching
#### Filter
   * GMS: Grid-based Motion Statistics for Fast, Ultra-Robust Feature Correspondence [[IJCV 2020]()] [[GMS-Feature-Matcher](https://github.com/JiawangBian/GMS-Feature-Matcher)]

   * Learning Two-View Correspondences and Geometry Using Order-Aware Network [[ICCV 2019](https://arxiv.org/pdf/1908.04964.pdf)] [[OANet](https://github.com/zjhthu/OANet)]
   
   * Learning to Find Good Correspondences [[CVPR 2018](https://openaccess.thecvf.com/content_cvpr_2018/papers/Yi_Learning_to_Find_CVPR_2018_paper.pdf)] [[learned-correspondence-release](https://github.com/vcg-uvic/learned-correspondence-release)]
 
   * ACNe: Attentive Context Normalization for Robust Permutation-Equivariant Learning [[CVPR 2020](https://openaccess.thecvf.com/content_CVPR_2020/papers/Sun_ACNe_Attentive_Context_Normalization_for_Robust_Permutation-Equivariant_Learning_CVPR_2020_paper.pdf)] [[acne](https://github.com/vcg-uvic/acne)]

   * Progressive Correspondence Pruning by Consensus Learning [[ICCV 2021](https://arxiv.org/pdf/2101.00591.pdf)] [[CLNet](https://github.com/sailor-z/CLNet)]

   * PGFNet: Preference-Guided Filtering Network for Two-View Correspondence Learning [[TIP 2023](https://ieeexplore.ieee.org/document/10041834)] [[PGFNet](https://github.com/guobaoxiao/PGFNet)]

   * Pentagon-Match (PMatch): Identification of View-Invariant Planar Feature for Local Feature Matching-Based Homography Estimation [[arXiv 2023](https://arxiv.org/pdf/2305.17463.pdf)] [[]()]

   * ConvMatch: Rethinking Network Design for Two-View Correspondence Learning [[AAAI 2023](https://openreview.net/pdf?id=DnaHIVXRzmh)] [[ConvMatch](https://github.com/SuhZhang/ConvMatch)]

   * Progressive Neighbor Consistency Mining for Correspondence Pruning [[CVPR 2023](https://openaccess.thecvf.com/content/CVPR2023/papers/Liu_Progressive_Neighbor_Consistency_Mining_for_Correspondence_Pruning_CVPR_2023_paper.pdf)] [[NCMNet](https://github.com/xinliu29/NCMNet)]


#### Matcher
   * SuperGlue: Learning Feature Matching with Graph Neural Networks [[CVPR 2020](https://arxiv.org/pdf/1911.11763.pdf)] [[SuperGluePretrainedNetwork](https://github.com/magicleap/SuperGluePretrainedNetwork)]

   * Learning to Match Features with Seeded Graph Matching Network [[ICCV 2021](https://arxiv.org/pdf/2108.08771.pdf)] [[SGMNet](https://github.com/vdvchen/SGMNet)]

   * ClusterGNN: Cluster-based Coarse-to-Fine Graph Neural Network for Efficient Feature Matching [[CVPR 2022](https://openaccess.thecvf.com/content/CVPR2022/papers/Shi_ClusterGNN_Cluster-Based_Coarse-To-Fine_Graph_Neural_Network_for_Efficient_Feature_Matching_CVPR_2022_paper.pdf)] [[]()]

   * AMatFormer: Efficient Feature Matching via Anchor Matching Transformer [[TMM 2023](https://arxiv.org/pdf/2305.19205.pdf)] [[]()]

   * :globe_with_meridians: SphereGlue: Learning Keypoint Matching on High Resolution Spherical Images [[CVPRW 2023](https://openaccess.thecvf.com/content/CVPR2023W/IMW/papers/Gava_SphereGlue_Learning_Keypoint_Matching_on_High_Resolution_Spherical_Images_CVPRW_2023_paper.pdf)] [[SphereGlue](https://github.com/vishalsharbidar/SphereGlue)]

   * LightGlue: Local Feature Matching at Light Speed [[ICCV 2023](https://arxiv.org/pdf/2306.13643v1.pdf)] [[LightGlue](https://github.com/cvg/LightGlue)]

   * ResMatch: Residual Attention Learning for Local Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2307.05180.pdf)] [[ResMatch](https://github.com/ACuOoOoO/ResMatch)]

   * IMP: Iterative Matching and Pose Estimation with Adaptive Pooling [[CVPR 2023](https://openaccess.thecvf.com/content/CVPR2023/papers/Xue_IMP_Iterative_Matching_and_Pose_Estimation_With_Adaptive_Pooling_CVPR_2023_paper.pdf)] [[imp-release](https://github.com/feixue94/imp-release)]

   * Scene-Aware Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2308.09949.pdf)] [[]()]
---
## Semi-dense

   * Neighbourhood Consensus Networks [[NeurIPS 2018](https://proceedings.neurips.cc/paper/2018/file/8f7d807e1f53eff5f9efbe5cb81090fb-Paper.pdf)] [[]()]

   * Efficient neighbourhood consensus networks via submanifold sparse convolutions [[ECCV 2020](https://arxiv.org/pdf/2004.10566.pdf)] [[sparse-ncnet](https://github.com/ignacio-rocco/sparse-ncnet)]

   * Dual-resolution correspondence networks [[NeurIPS 2020](https://proceedings.neurips.cc/paper/2020/file/c91591a8d461c2869b9f535ded3e213e-Paper.pdf)] [[]()] 

   * XResolution Correspondence Network [[BMVC 2021](https://arxiv.org/pdf/2012.09842.pdf)] [[xrcnet](https://github.com/XYZReality/xrcnet)]

   * Patch2Pix: Epipolar-Guided Pixel-Level Correspondences [[CVPR 2021](https://arxiv.org/pdf/2012.01909.pdf)] [[patch2pix](https://github.com/GrumpyZhou/patch2pix)]

   * DFM: A Performance Baseline for Deep Feature Matching [[CVPR 2021](https://arxiv.org/pdf/2106.07791.pdf)] [[DFM](https://github.com/ufukefe/DFM)]

   * LoFTR: Detector-Free Local Feature Matching with Transformers [[CVPR 2021](https://arxiv.org/pdf/2104.00680.pdf)] [[LoFTR](https://github.com/zju3dv/LoFTR)]

   * A case for using rotation invariant features in state of the art feature matchers [[CVPRW 2022](https://openaccess.thecvf.com/content/CVPR2022W/IMW/papers/Bokman_A_Case_for_Using_Rotation_Invariant_Features_in_State_of_CVPRW_2022_paper.pdf)] [[se2-loftr](https://github.com/inkyusa/se2-loftr)]

   * 3DG-STFM: 3D Geometric Guided Student-Teacher Feature Matching [[ECCV 2022](https://arxiv.org/pdf/2207.02375.pdf)] [[3DG-STFM](https://github.com/Ryan-prime/3DG-STFM)]

   * Local Feature Matching with Transformers for low-end devices [[arXiv 2022](https://arxiv.org/pdf/2202.00770.pdf)] [[Coarse_LoFTR_TRT](https://github.com/Kolkir/Coarse_LoFTR_TRT)]

   * QuadTree Attention for Vision Transformers [[ICLR 2022](https://arxiv.org/pdf/2201.02767.pdf)] [[QuadTreeAttention](https://github.com/Tangshitao/QuadTreeAttention)]

   * MatchFormer: Interleaving Attention in Transformers for Feature Matching [[ACCV 2022](https://arxiv.org/pdf/2203.09645.pdf)] [[MatchFormer](https://github.com/jamycheung/MatchFormer)]

   * ASpanFormer: Detector-Free Matching with Adaptive Span Transformer [[ECCV 2022](https://arxiv.org/pdf/2208.14201.pdf)] [[ml-aspanformer](https://github.com/apple/ml-aspanformer)]

   * TopicFM: Robust and Interpretable Topic-Assisted Feature Matching [[AAAI 2023](https://arxiv.org/pdf/2207.00328.pdf)] [[TopicFM](https://github.com/TruongKhang/TopicFM)]
   
   * DeepMatcher: A Deep Transformer-based Network for Robust and Accurate Local Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2301.02993v1.pdf)] [[DeepMatcher](https://github.com/XT-1997/DeepMatcher)]
   
   * OAMatcher: An Overlapping Areas-based Network for Accurate Local Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2302.05846.pdf)] [[OAMatcher](https://github.com/DK-HU/OAMatcher)]

   * PATS: Patch Area Transportation with Subdivision for Local Feature Matching [[CVPR 2023](https://arxiv.org/pdf/2303.07700.pdf)] [[pats](https://github.com/zju3dv/pats)]
   
   * PA-LoFTR: Local Feature Matching with 3D Position-Aware Transformer [[arXiv 2023](https://openreview.net/pdf?id=U8MtHLRK06q)] [[]()]
   
   * Improving Transformer-based Image Matching by Cascaded Capturing Spatially Informative Keypoints [[arXiv 2023](https://arxiv.org/pdf/2303.02885.pdf)] [[]()]
   
   * Structured Epipolar Matcher for Local Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2303.16646.pdf)] [[]()]

   * Adaptive Spot-Guided Transformer for Consistent Local Feature Matching [[CVPR 2023](https://arxiv.org/pdf/2303.16624.pdf)] [[astr](https://astr2023.github.io/)]
   
   * GlueStick: Robust Image Matching by Sticking Points and Lines Together [[ICCV 2023](https://arxiv.org/pdf/2304.02008v1.pdf)] [[GlueStick](https://github.com/cvg/GlueStick)]
   
   * E3CM: Epipolar-Constrained Cascade Correspondence Matching [[ssrn](https://deliverypdf.ssrn.com/delivery.php?ID=466101127096068115002104021110028109028027010042065026093047035108019046034025018076127124085118082122091102017004101067070000026084031074101107098016015007037090116038089124089041109039116122125126054094010014019119091093096019011031074029016031100089074070066098000006105073022119064086107&EXT=pdf&INDEX=TRUE)] [[]()]

  * MAIM: a mixer MLP architecture for image matching [[Unknown 2023](https://www.researchgate.net/publication/370365750_MAIM_a_mixer_MLP_architecture_for_image_matching)] [[]()]
 
 * Searching from Area to Point: A Hierarchical Framework for Semantic-Geometric Combined Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2305.00194.pdf)] [[]()]

 * Adaptive Assignment for Geometry Aware Local Feature Matching [[CVPR 2023](https://openaccess.thecvf.com/content/CVPR2023/papers/Huang_Adaptive_Assignment_for_Geometry_Aware_Local_Feature_Matching_CVPR_2023_paper.pdf)] [[AdaMatcher](https://github.com/TencentYoutuResearch/AdaMatcher)]

* TopicFM+: Boosting Accuracy and Efficiency of Topic-Assisted Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2307.00485.pdf)] [[TopicFM](https://github.com/TruongKhang/TopicFM)]

* TKwinFormer: Top k Window Attention in Vision Transformers for Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2308.15144.pdf)] [[TKwinFormer](https://github.com/LiaoYun0x0/TKwinFormer)]
   
* Occ2Net: Robust Image Matching Based on 3D Occupancy Estimation for Occluded Regions [[ICCV 2023](https://arxiv.org/pdf/2308.16160.pdf)] [[]()]

* FMRT: Learning Accurate Feature Matching with Reconciliatory Transformer [[arXiv 2023](https://arxiv.org/pdf/2310.13605.pdf)] [[]()]


## Dense

   * Dgc-net: Dense geometric correspondence network [[WACV 2019](https://arxiv.org/pdf/1810.08393.pdf)] [[DGC-Net](https://github.com/AaltoVision/DGC-Net)]

   * Ransac-flow: generic two-stage image alignment [[ECCV 2020](https://arxiv.org/pdf/2004.01526.pdf)] [[RANSAC-Flow](https://github.com/XiSHEN0220/RANSAC-Flow)]

   * GLU-Net: Global-local universal network for dense flow and correspondences [[CVPR 2020](https://openaccess.thecvf.com/content_CVPR_2020/papers/Truong_GLU-Net_Global-Local_Universal_Network_for_Dense_Flow_and_Correspondences_CVPR_2020_paper.pdf)] [[GLU-Net](https://github.com/PruneTruong/GLU-Net)]

   * DenseGAP: Graph-Structured Dense Correspondence Learning with Anchor Points [[ICPR 2022](https://arxiv.org/pdf/2112.06910.pdf)] [[DenseGAP](https://github.com/formyfamily/DenseGAP)]

   * Learning accurate dense correspondences and when to trust them [[CVPR 2021](https://openaccess.thecvf.com/content/CVPR2021/papers/Truong_Learning_Accurate_Dense_Correspondences_and_When_To_Trust_Them_CVPR_2021_paper.pdf)] [[PDCNet](https://github.com/PruneTruong/PDCNet)]

   * Pdc-net+: Enhanced probabilistic dense correspondence network [[arXiv 2021](https://arxiv.org/pdf/2109.13912.pdf)] [[DenseMatching](https://github.com/PruneTruong/DenseMatching)]

   * COTR: Correspondence Transformer for Matching Across Images [[ICCV 2021](https://openaccess.thecvf.com/content/ICCV2021/papers/Jiang_COTR_Correspondence_Transformer_for_Matching_Across_Images_ICCV_2021_paper.pdf)] [[COTR](https://github.com/ubc-vision/COTR)]

   * ECO-TR: Efficient Correspondences Finding Via Coarse-to-Fine Refinement [[ECCV 2022](https://arxiv.org/pdf/2209.12213.pdf)] [[ECO-TR](https://github.com/dltan7/ECO-TR)]
   
   * PUMP: Pyramidal and Uniqueness Matching Priors for Unsupervised Learning of Local Descriptors [[CVPR 2022](https://arxiv.org/pdf/2202.00667.pdf)] [[pump](https://github.com/naver/pump)]

   * DKM: Dense Kernelized Feature Matching for Geometry Estimation [[CVPR 2023](https://arxiv.org/pdf/2202.00667.pdf)] [[DKM](https://github.com/Parskatt/DKM)]

   * PMatch: Paired Masked Image Modeling for Dense Geometric Matching [[CVPR 2023](https://arxiv.org/pdf/2303.17342.pdf)] [[PMatch](https://github.com/ShngJZ/PMatch)]

   * RoMa: Revisiting Robust Losses for Dense Feature Matching [[arXiv 2023](https://arxiv.org/pdf/2305.15404.pdf)] [[RoMa](https://github.com/Parskatt/RoMa)]

   * RGM: A Robust Generalist Matching Model [[arXiv 2023](https://arxiv.org/pdf/2310.11755.pdf)] [[RGM](https://github.com/aim-uofa/RGM)]


---
## Pose estimation and others
   * :globe_with_meridians: Structure from motion using full spherical panoramic cameras [[ICCVW 2011](http://av.dfki.de/~pagani/papers/Pagani2011_OMNIVIS.pdf)] [[]()]

   * PoseNet: A Convolutional Network for Real-Time 6-DOF Camera Relocalization [[ICCV 2015](https://openaccess.thecvf.com/content_iccv_2015/papers/Kendall_PoseNet_A_Convolutional_ICCV_2015_paper.pdf)] [[PoseNet](https://github.com/crafterrr/PoseNet)]
     
   * Geometric loss functions for camera pose regression with deep learning [[CVPR 2017](https://openaccess.thecvf.com/content_cvpr_2017/papers/Kendall_Geometric_Loss_Functions_CVPR_2017_paper.pdf)] [[]()]
 
  * Relative Camera Pose Estimation Using Convolutional Neural Networks [[ACIVS 2017](https://arxiv.org/pdf/1702.01381.pdf)] [[relativeCameraPose](https://github.com/AaltoVision/relativeCameraPose)]

  * DSAC - Differentiable RANSAC for Camera Localization [[CVPR 2017](https://openaccess.thecvf.com/content_cvpr_2017/papers/Brachmann_DSAC_-_Differentiable_CVPR_2017_paper.pdf)] [[DSAC](https://github.com/cvlab-dresden/DSAC)]

  * Generalized Differentiable RANSAC [[arXiv 2022](https://www.researchgate.net/profile/Daniel-Barath/publication/366603570_Generalized_Differentiable_RANSAC/links/6422eea2a1b72772e431871a/Generalized-Differentiable-RANSAC.pdf)] [[differentiable_ransac](https://github.com/weitong8591/differentiable_ransac)]

   * RPNet: an End-to-End Network for Relative Camera Pose Estimation [[ECCVW 2018](https://openaccess.thecvf.com/content_ECCVW_2018/papers/11129/En_RPNet_an_End-to-End_Network_for_Relative_Camera_Pose_Estimation_ECCVW_2018_paper.pdf)] [[RPNet](https://github.com/ensv/RPNet)]

   * Camera relocalization by computing pairwise relative poses using convolutional neural network [[ICCVW 2017](https://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w17/Laskar_Camera_Relocalization_by_ICCV_2017_paper.pdf)] [[RelPoseNet](https://github.com/AaltoVision/RelPoseNet)]
   
   * Deep Keypoint-Based Camera Pose Estimation with Geometric Constraints [[IROS 2020](https://arxiv.org/pdf/2007.15122.pdf)] [[pytorch-deepFEPE](https://github.com/eric-yyjau/pytorch-deepFEPE)]
   
   * Wide-Baseline Relative Camera Pose Estimation with Directional Learning [[CVPR 2021](https://arxiv.org/pdf/2106.03336.pdf)] [[DirectionNet](https://github.com/arthurchen0518/DirectionNet)]

   * :globe_with_meridians: Robust 360-8PA: Redesigning The Normalized 8-point Algorithm for 360-FoV Images [[ICRA 2021](https://arxiv.org/pdf/2104.10900.pdf)] [[robust_360_8PA](https://github.com/EnriqueSolarte/robust_360_8PA)]

   * :globe_with_meridians: Pose Estimation for Two-View Panoramas: a Comparative Analysis [[CVPRW 2022](https://openaccess.thecvf.com/content/CVPR2022W/OmniCV/papers/Murrugarra-Llerena_Pose_Estimation_for_Two-View_Panoramas_Based_on_Keypoint_Matching_A_CVPRW_2022_paper.pdf)] [[Keypoints](https://github.com/Artcs1/Keypoints)]

   * The 8-Point Algorithm as an Inductive Bias for Relative Pose Prediction by ViTs [[3DV 2022](https://crockwell.github.io/rel_pose/data/paper.pdf)] [[rel_pose](https://github.com/crockwell/rel_pose)]

   * End2End Multi-View Feature Matching with Differentiable Pose Optimization [[ICCV 2023](https://openaccess.thecvf.com/content/ICCV2023/papers/Roessle_End2End_Multi-View_Feature_Matching_with_Differentiable_Pose_Optimization_ICCV_2023_paper.pdf)] [[e2e_multi_view_matching](https://github.com/barbararoessle/e2e_multi_view_matching)]

   * :globe_with_meridians: CoVisPose: Co-visibility Pose Transformer for Wide-Baseline Relative Pose Estimation in 360  Indoor Panoramas [[ECCV 2022](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136920610.pdf)] [[]()]

   * Map-free Visual Relocalization: Metric Pose Relative to a Single Image [[ECCV 2022](https://arxiv.org/pdf/2210.05494.pdf?trk=public_post_comment-text)] [[map-free-reloc](https://github.com/nianticlabs/map-free-reloc)]

   * :globe_with_meridians: GPR-Net: Multi-view Layout Estimation via a Geometry-aware Panorama Registration Network [[arXiv 2022](https://arxiv.org/pdf/2210.11419.pdf)] [[]()]

   * RelMobNet: End-to-end relative camera pose estimation using a robust two-stage training [[arXiv 2022](https://arxiv.org/pdf/2202.12838.pdf)] [[]()]
   
   * GRelPose: Generalizable End-to-End Relative Camera Pose Regression [[arXiv 2022](https://arxiv.org/pdf/2211.14950.pdf)] [[GRelPose](https://fadikhateeb.github.io/GRelPose/)]
         
   * A Lightweight Domain Adaptive Absolute Pose Regressor Using BARLOW TWINS Objective [[arXiv 2022](https://arxiv.org/pdf/2211.10963.pdf)] [[]()]
      
   * Uncertainty-Driven Dense Two-View Structure from Motion [[arXiv 2023](https://arxiv.org/pdf/2302.00523.pdf)] [[]()]
   
   * CGA-PoseNet: Camera Pose Regression via a 1D-Up Approach to Conformal Geometric Algebra [[arXiv 2023](https://arxiv.org/pdf/2302.05211.pdf)] [[]()]

   * :globe_with_meridians: Graph-CoVis: GNN-based Multi-view Panorama Global Pose Estimation [[arXiv 2023](https://arxiv.org/pdf/2304.13201.pdf)] [[]()]

---
## Similar images disambiguate
   * Doppelgangers: Learning to Disambiguate Images of Similar Structures [[ICCV 2023](https://arxiv.org/pdf/2309.02420.pdf)] [[Doppelgangers](https://github.com/RuojinCai/Doppelgangers)]

---
## Datasets
   * [HPatches](https://github.com/hpatches/hpatches-dataset)
   * [YFCC100M](https://multimediacommons.wordpress.com/yfcc100m-core-dataset/)
   * [MegaDepth](https://www.cs.cornell.edu/projects/megadepth/)
   * [ScanNet](http://www.scan-net.org/)
   * :globe_with_meridians: [Matterport3D](https://niessner.github.io/Matterport/)
   * :globe_with_meridians: [Zillow Indoor Dataset (ZInD)](https://github.com/zillow/zind)

---
## Challenges and workshops
   * [Image Matching Challenge 2023](https://www.kaggle.com/competitions/image-matching-challenge-2023)
   * [Image Matching Challenge 2022](https://www.kaggle.com/competitions/image-matching-challenge-2022/overview)
   * [Image Matching Challenge 2021](https://www.cs.ubc.ca/research/image-matching-challenge/current/)
   * [Image Matching Challenge 2020](https://www.cs.ubc.ca/research/image-matching-challenge/2020/)
   * [Image Matching Challenge 2019](https://image-matching-workshop.github.io/leaderboard/)
   * [Image Matching: Local Features and Beyond workshop at CVPR](https://image-matching-workshop.github.io/)
   * :globe_with_meridians: [Omnidirectional Computer Vision workshop at CVPR](https://sites.google.com/view/omnicv2022)

---
## Resources
* [image-matching-webui](https://github.com/Vincentqyw/image-matching-webui)

---
Format:
   * Title [[journal year]()] [[repo]()]
