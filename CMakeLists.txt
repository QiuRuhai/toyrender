cmake_minimum_required(VERSION 3.31)
project(RayTracing_In_One_Weekend)

set(CMAKE_CXX_STANDARD 14)

add_executable(RayTracing_In_One_Weekend
        main.cpp
        vec3.h
        color.h
        ray.h
        hittable.h
        sphere.h
        hittable_list.h
        rtweekend.h
        interval.h
        camera.h
        material.h
        aabb.h
        BVH.h
        texture.h
        rtw_stb_image.h
)
