# Apple Trailers Wrapper

![GitHub](https://img.shields.io/github/license/Puyodead1/AppleTrailersWrapper?style=plastic)
![PyPI - Python Version](https://img.shields.io/pypi/pyversions/AppleTrailersWrapper?style=plastic)
![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/Puyodead1/AppleTrailersWrapper?style=plastic)

Simple python package that wraps Apple Trailers<br>
PyPi: https://pypi.org/project/AppleTrailersWrapper/

Find the documentation at https://appletrailerswrapper.readthedocs.io/<br>
more information will be added to the docs soon


# Example
```py
import AppleTrailersWrapper

results = AppleTrailersWrapper.Search("Allegiant") # Search for a title (see the search page of docs for format of JSON response)
title = AppleTrailersWrapper.Title(results["results"][0]) # Create instance of Title, passing a result dict

movie_title = title.get_movie_title()
print(movie_title)
```
