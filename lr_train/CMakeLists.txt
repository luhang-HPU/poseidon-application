cmake_minimum_required(VERSION 3.12)

add_executable(test_ckks_lrtrain test_ckks_lrtrain.cpp)
target_link_libraries(test_ckks_lrtrain poseidon_shared)

add_executable(ckks_lrtrain_opt ckks_lrtrain_opt.cpp batch_handler.h batch_handler.cpp)
target_link_libraries(ckks_lrtrain_opt poseidon_shared)
