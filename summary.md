Summary
- BooleanOperatorsTest

    1. should_perform_logical_boolean_operations
    2. should_do_bitwise_and_boolean_operation
    3. should_do_bitwise_or_boolean_operation
    4. should_do_bitwise_not_operation

    Q1: What is the knowledge point of the test? Where is the official document to the knowledge point?
    A1: To learn of the behaviors of basic boolean and bitwise operation and be able to use them.

    Q2: Why the test failed at first?
    A2: Because the expected values are not set.

    Q3: Why you corrected the test that way?
    A3: Tests [1-4] - I solved the results by performing boolean & bitwise operations and then added the result to the expected output.

    Q4: Do you have further questions on this knowledge point?
    A4: None

- CharTypeTest

    1. should_describe_escaped_chars

    Q1: What is the knowledge point of the test? Where is the official document to the knowledge point?
    A1: To learn of the characters that needs to be escaped before it can be used.
    
    Q2: Why the test failed at first?
    A2: Because the expected values are not set.

    Q3: Why you corrected the test that way?
    A3: I added the corresponding escaped characters to the expected outputs.

    Q4: Do you have further questions on this knowledge point?
    A4: None

- FloatingTypeTest

    1. should_not_get_rounded_result_if_convert_floating_number_to_integer
    3. should_not_round_number_when_convert_to_integer
    2. should_judge_special_double_cases
    4. should_round_number

    Q1: What is the knowledge point of the test? Where is the official document to the knowledge point?
    A1: To learn about how java handles convertion of primitive float and double types and make use of existing functions defined in object classes. 
    
    Q2: Why the test failed at first?
    A2: Because the expected values are not set.

    Q3: Why you corrected the test that way?
    A3: Tests [1-2] - Converting float to integer will disregard the decimal value. I added 2 as the expected result. 
    Test [3] - There are existing methods from the Double class which are Double.isNan & Double.isInfinite that returns the expected results. I completed the methods by making use of these functions.
    Test [4] - There is an existing method from the Math class which rounds the value of the number. I just used it to get the expected result. 

    Q4: Do you have further questions on this knowledge point?
    A4: None

- IntegerTypeTest

    1. should_get_range_of_primitive_int_type
    2. should_get_range_of_primitive_short_type
    3. should_get_range_of_primitive_long_type
    4. should_get_range_of_primitive_byte_type
    5. should_overflow_silently
    6. should_underflow_silently
    7. should_throw_exception_when_overflow
    8. should_take_care_of_number_type_when_doing_calculation
    9. should_truncate_number_when_casting
    10. should_increment
    11. should_increment_2

    Q1: What is the knowledge point of the test? Where is the official document to the knowledge point?
    A1: To learn and make use of existing constants and functions defined in object classes, to know what would occur when an integer overflows or underflows, to know the difference of arithmetic operations on integers and doubles/floats, to differentiate the amount of bits an integer has from a short or long variable, to learn of the effects of post- and pre- incrementing a value.
    
    Q2: Why the test failed at first?
    A2: Because the expected values are not set.

    Q3: Why you corrected the test that way?
    A3: Tests [1-4] - There are existing MAX & MIN constants defined in their respective classes. I just used it to get the expected results.
    Tests [5-6] - When integer overflow occurs it will result to the minimum value of integer, while integer underflow will result to the maximum value of integer. 
    Test [7] - There is an existing function in the Math class which is Math.addExact that adds two numbers and would throw an exception when it overflows. I completed the method by using this function.
    Test[8] - The values used are integers so it would do operations as such. For the 1st result: 2 / 3 = 0; 0 * 5 = 0, for the 2nd result: 2 * 5 = 10; 10 / 3 = 3.
    Test[9] - Short has a lower amount of bits than an integer, so it would truncate the values greater than 16 bits. I added 0x4567 as the expected result.
    Test[10-11] - Post-incrementing will return the value first then increment the value, while Pre-incrementing will increment the value then return it.

    Q4: Do you have further questions on this knowledge point?
    A4: None