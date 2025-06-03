# Changelog

## [1.11.0] - 2024-03-19

### Added
- Support for including linked markdown files in PDF exports
- Recursive processing of linked files
- Hierarchical structure preservation in exported PDFs
- Page breaks between linked files
- Proper heading level adjustment for linked content

### Modified
- Updated file processing logic to handle linked files
- Enhanced document merging to maintain structure
- Improved heading hierarchy in merged documents
- Added source file tracking in merged content

### Technical Details
- Implemented breadth-first processing of linked files
- Added file tracking to prevent infinite recursion
- Enhanced document merging with proper section handling
- Added source file information as data attributes
- Improved heading level management for linked content

## Implementation Details

### File Processing
- Files are processed in breadth-first order to maintain hierarchy
- Each file is processed only once to prevent duplicates
- Linked files are tracked to prevent infinite recursion

### Document Structure
- Each linked file starts on a new page
- Headers are adjusted to maintain proper hierarchy
- Source file information is preserved in data attributes
- Original document structure is maintained

### PDF Export
- All linked content is included in the final PDF
- Proper page breaks between files
- Maintained formatting and styling
- Preserved document hierarchy 