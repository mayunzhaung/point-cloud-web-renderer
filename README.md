
# Point cloud web renderer


Point clouds are an efficient way to represent 3D models. A significant amount of interest has emerged for this type of visual data, due to the recent advances in acquisition and compression technologies. However, adequate rendering solutions to display high-quality point cloud models, are still not openly available.

In this project, a web-based renderer is developed on top of the well-established **three.js** library, ensuring compatibility across different devices and operating systems. The renderer supports visualization of point clouds with real-time interaction, while rendering parameters and viewing conditions can be easily configured. The user is able to choose between either an adaptive, or a fixed splat size rendering mode in order to display the models. The renderer supports both PLY and PCD point cloud file formats. The current settings have been optimized for voxelized contents, without this limiting its usage, though. The source code is made publicly open for potential extensions and refinements.

In this repository, three applications of the point cloud renderer are provided. In particular:
- **pointCloudViewer**: Standalone viewer of a single point cloud model. Several models can be sequentially displayed, if specified by the user.
- **pointCloudQualityAssessmentTestbed**: Side-by-side viewer of point clouds, including annotation of the models and a panel for rating. This testbed was used for the subjective evaluations of [1].
- **pointCloudViewGrabber**: Tool to either reproduce the session of a user, or to display pre-defined views of a model. This tool was used to obtain projections of the point clouds under assessment before computing the projection-based metrics in [1].


Additional folders:
- **assets**: Contains two sub-folders, namely, models and pointsize. The former contains the point cloud models under inspection, while the latter carries meta-data files related to the point size of each model.
- **three.js**: Dependency of the software.

The selection of point cloud models, the rendering mode, the display settings, and the interactivity parameters can be adjusted through configuration files for each application. Examples of usage are provided. Below, a screenshot of the testbed is illustrated:

![alt text](/docs/screenshot.png)


### Conditions of use

If you wish to use this software in your research, please cite [1].


### References

[1] Alexiou, E., Viola, I., Borges, T., Fonseca, T., De Queiroz, R., & Ebrahimi, T. (2019). A comprehensive study of the rate-distortion performance in MPEG point cloud compression. APSIPA Transactions on Signal and Information Processing, 8, E27. doi:10.1017/ATSIP.2019.20
