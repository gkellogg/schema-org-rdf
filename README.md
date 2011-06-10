# Schema.org in RDF

This is a project to provide an RDF(S) version of Schema.org including tools to benefit from data that uses Schema.org terms.


## Who is behind this?

The EC FP7  LOD-Around-The-Clock Support Action (<a href="http://latc-project.eu/">LATC</a>) and people from the Linked Data Research Centre, [DERI](http://www.deri.ie).

## License

This software is Public Domain.


## Generating the RDF and other versions

Run the following Python scripts in the `scrapers` directory:

    scrape_rdf.py
    scrape_json.py
    scrape_csv.py

They either write to STDOUT or to a filename taken as command
line argument.

There is also a script that generates all formats, does a bit
of sanity checking to see if it worked, and copies them to a
target directory. 

    cd scrapers
    ./run.rb temp-directory target-directory

This requires the any23 command line tool on the path.
