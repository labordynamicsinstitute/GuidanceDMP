# DMP guidance

There are a variety of tools to assist building data management plans. Start with https://dmp.cdlib.org/, or consult your local RESEARCH DATA MANAGEMENT SERVICE GROUP (titles may vary).

Generically, the question you will want to ask yourself are (source: http://data.research.cornell.edu/content/data-management-planning)

## Data types and sources
> What types of data, samples, physical collections, code, software, curriculum materials and other materials will be produced in the course of the project?

- Note that computer code/programs/software are part of a data management plan. Many DMP have been observed that state "no data is being generated" when in fact computer code or documents are being created.
- Note that this also encompasses video.

## Formats and standards
> What standards will be used for your files and metadata?

You want to express things in terms of "ASCII" or "UTF-8", PDF. Most computer code is straight ASCII, but compiled objects may not themselves be in compliant formats. Avoid archiving data as "native" formats (Stata, SPSS, etc.), though some are better then others (hint: if you can find open-source converters, say in R or python, that can read the format without needing external software, then it might be OK).

A useful guide may be here:
http://guides.library.cornell.edu/ecommons/formats

## Roles and responsibilities
> What are the roles and who has responsibilities for managing data?

For simple proposals, this will be the PI, but for bigger projects, there might be a designated manager for this. Also check to see if your library provides support on this.

## Dissemination methods
> What are the methods for sharing data and metadata during and after the award period?

NOTES:
- A project or personal website is acceptable during the award period. However, after the award period, such websites should be considered ephemeral. Using archives (see below) is one alternative for after the award period (dissemination and preservation often go hand-in-hand).
- Posting to software archives (Github, Gitlab, Bitbucket, etc.), Youtube, etc. is acceptable during the award period.

## Policies for public access, data sharing, and re-use
> How will you meet funder requirements to provide public access to your data while protecting privacy, confidentiality, security and intellectual property rights?

NOTES: This usually means specifying some sort of license for re-use, which may be open-source or not. It is possible to closed-source license objects with a free license for certain types of users, such as the government.

## Preservation
> How will you preserve the integrity of your data over time?

NOTES:
- This includes converting to preservation-friendly formats, see f.i. http://guides.library.cornell.edu/ecommons/formats

- Most universities have libraries or archives on-campus that are able to fulfill that role. Sample statements might be (source: http://guides.library.cornell.edu/ecommons/datapolicy)

>   [Specify datasets] will be deposited in [University Library]'s institutional
    repository, [NAME OF REPOSITORY (http://dspace.myuniversity.edu)], for
    preservation and access. Datasets will be available via the world wide web without
    restriction. The repository provides each item with a persistent URL and is
    committed to preserving the binary form of the digital object.

- Storing data on shared drives or filesystem does not qualify as preservation. Preservation implies an active effort, typically exerted by librarians or archivists, whose job it is to worry about migrating (occasionally) from one archive to a new one. Shared drives or filesystems (university-provided or commercial) do not do that. They also do not provide persistent URLs.

- Journals sometimes fulfill this role, but only for accepted and published articles. Not all journals do so. Not all documents and files produced by a project will be accepted or published, but all documents and files need to be covered by the DMP.

- A personal website never qualifies, even if you have tenure.

- Github and similar sites do not qualify as preservation sites on their own!

- Examples of dissemination and preservation tools:
  - Github (for dissemination of code) combined with Zenodo (an archive with hooks into Github) https://guides.github.com/activities/citable-code/
  - Open Science Framework (http://osf.io) does both versioning and archiving.
  - Private versioning system with embargoed archives on a university "dspace" or "ecommons" instance (manual upload).
  - Using `httrack` (https://www.httrack.com/) to make an offline copy of a project website and archive it at a university archive.
  - Posting videos on Youtube, then downloading them in MPEG-4 (H.263, H.264) format and archiving on a university archive.
  - Uploading large datasets to (open)ICPSR (http://openicpsr.org, http://www.icpsr.umich.edu), Harvard Dataverse (http://dataverse.harvard.edu), Zenodo (http://zenodo.org)
