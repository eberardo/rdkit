rdkit_python_extension(rdMMPA
                       rdMMPA.cpp
                       DEST Chem
                       LINK_LIBRARIES MMPA
SubstructMatch SmilesParse GraphMol DataStructs RDGeometryLib RDGeneral 
RDBoost )

add_pytest(pyMMPA ${CMAKE_CURRENT_SOURCE_DIR}/testMMPA.py)
