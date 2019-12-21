from ct:18.04

COPY ct ct
RUN cd ct && mkdir build && cd build && cmake .. && make

WORKDIR /workspace/ct/build/tests
RUN reflect/test_ct_get_name
RUN reflect/test_ct_reflect_access
RUN reflect/test_ct_reflect_compare
RUN reflect/test_ct_reflect_hash
RUN reflect/test_ct_reflect_print
RUN reflect/test_ct_static_checks
RUN reflect/test_ct_data_table
RUN enum/test_ct_enum
RUN enum/test_ct_enum_cuda
RUN string/test_ct_string_runtime
RUN string/test_ct_string_static
RUN variadic_typedef/test_ct_variadic_typedef
RUN type_trait_detectors/test_ct_type_traits
RUN hash/test_ct_string_hash
