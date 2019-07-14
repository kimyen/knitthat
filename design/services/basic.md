# Basic Services

## Track Yarn Stash

## Track Needle Stash

## Track Project

## Design a Project

| Method | Path     | Request Object | Response Object |
|--------|----------|----------------|-----------------|
| POST   | /row     | Row            | Row             |
| POST   | /piece   | Piece          | Piece           |
| POST   | /project | Project        | Project         |

## Browse

| Method | Path          | Path Parameters | Response Object |
|--------|---------------|-----------------|-----------------|
| GET    | /projects     | nextPageToken   | ProjectPage     |
| GET    | /project/{id} |                 | Project         |
| GET    | /piece/{id}   |                 | Piece           |
| GET    | /row/{id}     |                 | Row             |
| GET    | /stats        |                 | Stats           |

## Objects

| ProjectPage                   |
|-------------------------------|
| List of Integer projectIdList |
| String nextPageToken          |

| Project                     |
| ----------------------------|
| String name                 |
| Integer id                  |
| Date createdOn              |
| Date modifiedOn             |
| Integer createdBy           |
| Integer modifiedBy          |
| List of Integer pieceIdList |

| Piece                     |
| --------------------------|
| String name               |
| Integer id                |
| Date createdOn            |
| Date modifiedOn           |
| Integer createdBy         |
| Integer modifiedBy        |
| List of Integer rowIdList |

| Row                     |
| ------------------------|
| String name             |
| Integer id              |
| Date createdOn          |
| Date modifiedOn         |
| Integer createdBy       |
| Integer modifiedBy      |
| List of Enum stitchList |
  
| Stats                    |
| -------------------------|
| Integer finishedProjects |
| Integer finishedStitches |
