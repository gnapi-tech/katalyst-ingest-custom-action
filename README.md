Katalyst Test Ingest Action
This action uploads JUnit and LCOV reports to the Katalyst ingestion API.

Inputs
katalyst_base_url - required
ingest_token - required
project_id - required
junit_path - optional, default junit.xml
lcov_path - optional, default coverage/lcov.info
Example
- uses: gnapi-shared/katalyst-ingest-action@v1
  with:
      katalyst_base_url: ${{ secrets.KATALYST_BASE_URL }}
      ingest_token: ${{ secrets.KATALYST_INGEST_TOKEN }}
      project_id: ${{ secrets.KATALYST_PROJECT_ID }}
