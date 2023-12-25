cmake_minimum_required(VERSION 3.15)

include(proj.conf)

find_package(bouffalo_sdk REQUIRED HINTS $ENV{BL_SDK_BASE})

sdk_set_main_file(main.c)

sdk_add_static_library(/home/wei/rtthread-rs/target/riscv64gc-sipeed-freertos/release/librtthread_rs.a)

project(helloworld)
