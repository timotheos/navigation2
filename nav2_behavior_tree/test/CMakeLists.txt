ament_add_gtest(test_decorator_distance_controller
  plugins/decorator/test_distance_controller.cpp
)
target_link_libraries(test_decorator_distance_controller
  nav2_distance_controller_bt_node
)
ament_target_dependencies(test_decorator_distance_controller
  ${dependencies}
)

ament_add_gtest(test_condition_distance_traveled
  plugins/condition/test_distance_traveled.cpp
)
target_link_libraries(test_condition_distance_traveled
  nav2_distance_traveled_condition_bt_node
)
ament_target_dependencies(test_condition_distance_traveled
  ${dependencies}
)

ament_add_gtest(test_condition_time_expired
  plugins/condition/test_time_expired.cpp
)
target_link_libraries(test_condition_time_expired
  nav2_time_expired_condition_bt_node
)
ament_target_dependencies(test_condition_time_expired
  ${dependencies}
)
