
add_definitions(-DTHIS_SOURCE_DIR="${CMAKE_CURRENT_SOURCE_DIR}")

add_executable(openMVG_sample_multiview_robustEssential_spherical robust_essential_spherical.cpp)
target_link_libraries(openMVG_sample_multiview_robustEssential_spherical
  openMVG_image
  openMVG_multiview
  openMVG_features
  openMVG_matching
  openMVG_system
  openMVG_sfm
  stlplus
  vlsift
  )

set_property(TARGET openMVG_sample_multiview_robustEssential_spherical PROPERTY FOLDER OpenMVG/Samples)

