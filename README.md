Simple example of couroutines.

Ubuntu 20.04

    gcc (Ubuntu 10.3.0-1ubuntu1~20.04) 10.3.0
    Copyright (C) 2020 Free Software Foundation, Inc.
    This is free software; see the source for copying conditions.  There is NO
    warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

Using `-fcoroutines -std=gnu++2a`

inspired: https://www.modernescpp.com/index.php/an-infinite-data-stream-with-coroutines-in-c-20

result:

    getNext():            promise_type::promise_type
    promise_type::get_return_object
    Generator::Generator
    promise_type::initial_suspend
    Generator::getNextValue
    promise_type::yield_value
    0         Generator::getNextValue
    promise_type::yield_value
    1         Generator::getNextValue
    promise_type::yield_value
    2         Generator::getNextValue
    promise_type::yield_value
    3         Generator::getNextValue
    promise_type::yield_value
    4         Generator::getNextValue
    promise_type::yield_value
    5         Generator::getNextValue
    promise_type::yield_value
    6         Generator::getNextValue
    promise_type::yield_value
    7         Generator::getNextValue
    promise_type::yield_value
    8         Generator::getNextValue
    promise_type::yield_value
    9         Generator::getNextValue
    promise_type::yield_value
    10
    
    getNext(100, -10):            promise_type::promise_type
    promise_type::get_return_object
    Generator::Generator
    promise_type::initial_suspend
    Generator::getNextValue
    promise_type::yield_value
    100         Generator::getNextValue
    promise_type::yield_value
    90         Generator::getNextValue
    promise_type::yield_value
    80         Generator::getNextValue
    promise_type::yield_value
    70         Generator::getNextValue
    promise_type::yield_value
    60         Generator::getNextValue
    promise_type::yield_value
    50         Generator::getNextValue
    promise_type::yield_value
    40         Generator::getNextValue
    promise_type::yield_value
    30         Generator::getNextValue
    promise_type::yield_value
    20         Generator::getNextValue
    promise_type::yield_value
    10         Generator::getNextValue
    promise_type::yield_value
    0         Generator::getNextValue
    promise_type::yield_value
    -10         Generator::getNextValue
    promise_type::yield_value
    -20         Generator::getNextValue
    promise_type::yield_value
    -30         Generator::getNextValue
    promise_type::yield_value
    -40         Generator::getNextValue
    promise_type::yield_value
    -50         Generator::getNextValue
    promise_type::yield_value
    -60         Generator::getNextValue
    promise_type::yield_value
    -70         Generator::getNextValue
    promise_type::yield_value
    -80         Generator::getNextValue
    promise_type::yield_value
    -90         Generator::getNextValue
    promise_type::yield_value
    -100
    Generator::~Generator
    promise_type::~promise_type
    Generator::~Generator
    promise_type::~promise_type
