cmake_minimum_required(VERSION 3.10)

project(usbhost)

include_directories(include/)

add_library(
    usbhost
    src/usbhost.c
)
