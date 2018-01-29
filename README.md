# KeyedFrames

[![Stable](https://img.shields.io/badge/docs-stable-blue.svg)](https://invenia.github.io/KeyedFrames.jl/stable)
[![Latest](https://img.shields.io/badge/docs-latest-blue.svg)](https://invenia.github.io/KeyedFrames.jl/latest)
[![Build Status](https://travis-ci.org/invenia/KeyedFrames.jl.svg?branch=master)](https://travis-ci.org/invenia/KeyedFrames.jl)
[![Build Status](https://ci.appveyor.com/api/projects/status/github/invenia/KeyedFrames.jl?svg=true)](https://ci.appveyor.com/project/invenia/KeyedFrames-jl)
[![CodeCov](https://codecov.io/gh/invenia/KeyedFrames.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/invenia/KeyedFrames.jl)

A `KeyedFrame` is a `DataFrame` that also stores a vector of column names that together act
as a unique key.

When a `KeyedFrame` is joined with another `KeyedFrame` (or any other `AbstractDataFrame`),
the key can be used to determine which columns to join on. When a `KeyedFrame` is sorted, it
will sort by the key columns first by default.
