set(Module_SRCS
  vtkRTXMLPolyDataReader.cxx
  vtkXMLCompositeDataReader.cxx
  vtkXMLCompositeDataWriter.cxx
  vtkXMLDataReader.cxx
  vtkXMLDataSetWriter.cxx
  vtkXMLFileReadTester.cxx
  vtkXMLGenericDataObjectReader.cxx
  vtkXMLHierarchicalBoxDataFileConverter.cxx
  vtkXMLHierarchicalBoxDataReader.cxx
  vtkXMLHierarchicalBoxDataWriter.cxx
  vtkXMLHierarchicalDataReader.cxx
  vtkXMLHyperOctreeReader.cxx
  vtkXMLHyperOctreeWriter.cxx
  vtkXMLImageDataReader.cxx
  vtkXMLImageDataWriter.cxx
  vtkXMLMultiBlockDataReader.cxx
  vtkXMLMultiBlockDataWriter.cxx
  vtkXMLMultiGroupDataReader.cxx
  vtkXMLPDataReader.cxx
  vtkXMLPImageDataReader.cxx
  vtkXMLPolyDataReader.cxx
  vtkXMLPolyDataWriter.cxx
  vtkXMLPPolyDataReader.cxx
  vtkXMLPRectilinearGridReader.cxx
  vtkXMLPStructuredDataReader.cxx
  vtkXMLPStructuredGridReader.cxx
  vtkXMLPUnstructuredDataReader.cxx
  vtkXMLPUnstructuredGridReader.cxx
  vtkXMLReader.cxx
  vtkXMLRectilinearGridReader.cxx
  vtkXMLRectilinearGridWriter.cxx
  vtkXMLStructuredDataReader.cxx
  vtkXMLStructuredDataWriter.cxx
  vtkXMLStructuredGridReader.cxx
  vtkXMLStructuredGridWriter.cxx
  vtkXMLUniformGridAMRReader.cxx
  vtkXMLUniformGridAMRWriter.cxx
  vtkXMLUnstructuredDataReader.cxx
  vtkXMLUnstructuredDataWriter.cxx
  vtkXMLUnstructuredGridReader.cxx
  vtkXMLUnstructuredGridWriter.cxx
  vtkXMLWriterC.cxx
  vtkXMLWriter.cxx
  )

set_source_files_properties(
  vtkXMLCompositeDataReader
  vtkXMLCompositeDataWriter
  vtkXMLDataReader
  vtkXMLPDataReader
  vtkXMLPStructuredDataReader
  vtkXMLPUnstructuredDataReader
  vtkXMLReader
  vtkXMLStructuredDataReader
  vtkXMLStructuredDataWriter
  vtkXMLUnstructuredDataReader
  vtkXMLUnstructuredDataWriter
  vtkXMLWriter
  ABSTRACT
  )

set_source_files_properties(
  vtkXMLWriterC
  WRAP_EXCLUDE
  )

vtk_module_library(vtkIOXML ${Module_SRCS})
