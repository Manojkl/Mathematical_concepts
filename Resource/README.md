# C++ libraries that support Numpy like operations.

* The [GNU Scientific Library](http://www.gnu.org/software/gsl/) is a GPL software written in C. Thus, it has a C-like allocation and way of programming (pointers, etc.). With the [GSLwrap](http://gslwrap.sourceforge.net/), you can have a C++ way of programming, while still using the GSL. GSL has a [BLAS](http://en.wikipedia.org/wiki/Basic_Linear_Algebra_Subprograms) implementation, but you can use [ATLAS](http://math-atlas.sourceforge.net/) instead of the default CBLAS, if you want even more performances.

* The [boost/uBLAS](http://www.boost.org/doc/libs/1_49_0/libs/numeric/ublas/doc/index.htm) library is a BSL library, written in C++ and distributed as a boost package. It is a C++-way of implementing the BLAS standard. uBLAS comes with a few linear algebra functions, and there is an [experimental binding to ATLAS](http://www.crystalclearsoftware.com/cgi-bin/boost_wiki/wiki.pl?Linear_Algebra_With_UBLAS).

* [eigen](http://eigen.tuxfamily.org/) is a linear algebra library written in C++, distributed under the LGPL3 (or GPL2). It's a C++ way of programming, but more integrated than the two others (more algorithms and data structures are available). Eigen [claim to be faster](http://eigen.tuxfamily.org/index.php?title=FAQ#How_does_Eigen_compare_to_BLAS.2FLAPACK.3F) than the BLAS implementations above, while not following the de-facto standard BLAS API. Eigen does not seem to put a lot of effort on parallel implementation.

* [Armadillo](http://arma.sourceforge.net/) is LGPL3 library for C++. It has binding for [LAPACK](http://www.netlib.org/lapack/) (the library used by numpy). It uses recursive templates and template meta-programming, which is a good point.

* [xtensor](https://github.com/QuantStack/xtensor) is a C++ library that is BSD licensed. It offers A C++ API very similar to that of NumPy. See https://xtensor.readthedocs.io/en/latest/numpy.html for a cheat sheet.
