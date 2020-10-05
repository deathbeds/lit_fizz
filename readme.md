# fizzbuzz literate program

a fizzbuzz program written as a literate program.

## developer

    def task_book():

build a book with [jupyter book] based on the `"_toc.yml" and "_config.yml" configuration files.

        return dict(actions=["jb build ."], file_dep=["_toc.yml"], targets=["_build/html"])

    def task_pdf():
        return dict(actions=["jb build . --builder pdfhtml"], file_dep=['_toc.yml'], targets=['_build/pdf/book.pdf'])
