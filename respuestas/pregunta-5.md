MATCH path = (a:Persona)-[:AMIGO_DE*]->(b:Persona)
WHERE ALL(rel IN relationships(path) WHERE rel.since > 2018)
RETURN path