cmake_minimum_required(VERSION 3.5)
project(node_with_subscription)

find_package(ros_cmake_auto REQUIRED)
ros_cmake_auto_alias_to_rca()

rca_start(LANGUAGES c++ CPP_STD c++14)

rca_add_node(node_with_subscription CLASS_NAME NodeWithSubscription src/node_with_subscription.cpp)

rca_end()
