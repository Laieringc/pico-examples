add_executable(test
        test.c
        )

# Pull in our pico_stdlib which pulls in commonly used features
target_link_libraries(test pico_stdlib)

# create map/bin/hex file etc.
pico_add_extra_outputs(test)

# add url via pico_set_program_url
example_auto_set_url(test)
