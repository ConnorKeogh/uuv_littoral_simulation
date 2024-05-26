find_package(gazebo REQUIRED)

set (worlds
  HTide_NObstacles.world  
  HTide_LObstacles.world
  HTide_HObstacles.world
  LTide_NObstacles.world  
  LTide_LObstacles.world
  LTide_HObstacles.world
)

# Install all the world files
install(FILES ${worlds}
  DESTINATION ${CMAKE_INSTALL_PREFIX}/share/gazebo-${GAZEBO_VERSION}/worlds)
