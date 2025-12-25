cmake_minimum_required(VERSION 3.18)
project(RayTracing_In_One_Weekend)

set(CMAKE_CXX_STANDARD 17)

add_executable(toyrenderer
        core/main.cpp
        core/vec3.h
        core/color.h
        core/ray.h
        core/hittable.h
        core/sphere.h
        core/hittable_list.h
        core/rtweekend.h
        core/interval.h
        core/camera.h
        core/material.h
        core/aabb.h
        core/BVH.h
        core/texture.h
        core/rtw_stb_image.h
        core/perlin.h
        core/quad.h
        core/constant_medium.h
        core/onb.h
        core/pdf.h
)    

find_package(OpenMP REQUIRED)
if(OpenMP_CXX_FOUND)
    target_link_libraries(toyrenderer PUBLIC OpenMP::OpenMP_CXX)
endif()
