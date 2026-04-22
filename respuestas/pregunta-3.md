MATCH (p:Persona)-[:USA_TECNOLOGIA]->(t:Tecnologia)
RETURN p.nombre, collect(t.nombre) AS tecnologias