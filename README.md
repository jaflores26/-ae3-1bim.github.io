# -ae3-1bim.github.io
ALTER TABLE `Director de Cine` ADD COLUMN 	`Field2`	INTEGER
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
ALTER TABLE `Director de Cine` ADD COLUMN 	`Field3`	INTEGER
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	INTEGER,
	`Field3`	INTEGER
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	INTEGER
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
ALTER TABLE `Director de Cine` ADD COLUMN 	`Field4`	INTEGER
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años,
	PRIMARY KEY(`Field1`)
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
SELECT COUNT(*) FROM (SELECT COUNT(`_rowid_`) FROM `Director de Cine` WHERE `Field1` IS NULL);
SELECT COUNT(`_rowid_`) FROM `Director de Cine` WHERE `Field1` IS NULL LIMIT 0, 50000;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre NOT NULL,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años,
	PRIMARY KEY(`Field1`)
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años,
	PRIMARY KEY(`Field1`)
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
SELECT COUNT(*) FROM (SELECT COUNT(*) FROM `Director de Cine` WHERE `Field1` <> CAST(`Field1` AS INTEGER));
SELECT COUNT(*) FROM `Director de Cine` WHERE `Field1` <> CAST(`Field1` AS INTEGER) LIMIT 0, 50000;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años,
	PRIMARY KEY(`Field1`)
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre PRIMARY KEY AUTOINCREMENT,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años
);
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
SELECT COUNT(*) FROM (SELECT COUNT(*) FROM `Director de Cine` WHERE `Field1` <> CAST(`Field1` AS INTEGER));
SELECT COUNT(*) FROM `Director de Cine` WHERE `Field1` <> CAST(`Field1` AS INTEGER) LIMIT 0, 50000;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años,
	PRIMARY KEY(`Field1`)
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre PRIMARY KEY AUTOINCREMENT,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años
);
SELECT COUNT(*) FROM (SELECT COUNT(`Field1`) FROM `Director de Cine`);
SELECT COUNT(`Field1`) FROM `Director de Cine` LIMIT 0, 50000;
SELECT COUNT(*) FROM (SELECT COUNT(DISTINCT `Field1`) FROM `Director de Cine`);
SELECT COUNT(DISTINCT `Field1`) FROM `Director de Cine` LIMIT 0, 50000;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre PRIMARY KEY AUTOINCREMENT UNIQUE,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años
);
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre UNIQUE,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años,
	PRIMARY KEY(`Field1`)
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre UNIQUE,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	apellido,
	`Field3`	nacionalidad,
	`Field4`	experiencia en años
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Director de Cine`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Director de Cine`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Director de Cine`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	
 

Dadas dos entidades:

Director de Cine:
nombre

apellido

nacionalidad

experiencia en años

Película
nombre
);
ALTER TABLE `Película` ADD COLUMN 	`Field2`	INTEGER
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
ALTER TABLE `Película` ADD COLUMN 	`Field3`	INTEGER
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
ALTER TABLE `Película` ADD COLUMN 	`Field4`	INTEGER
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
ALTER TABLE `Película` ADD COLUMN 	`Field5`	INTEGER
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	TEXT,
	`Field4`	costo de película,
	`Field5`	INTEGER
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	TEXT,
	`Field4`	costo de película,
	`Field5`	INTEGER
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	TEXT,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	INTEGER,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	
 

Dadas dos entidades:

Director de Cine:
nombre

apellido

nacionalidad

experiencia en años

Película
nombre,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	
 

Dadas dos entidades:

Director de Cine:
nombre

apellido

nacionalidad

experiencia en años

Película
nombre,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	tipo de película,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	BLOB,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	BLOB,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	REAL,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	REAL,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	NUMERIC,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	NUMERIC,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	INTEGER,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	TEXT,
	`Field2`	INTEGER,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	INTEGER,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	TEXT,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	BLOB,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	REAL,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	BLOB,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	TEXT,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	INTEGER,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master;
CREATE TABLE `sqlitebrowser_rename_column_new_table` (
	`Field1`	nombre,
	`Field2`	INTEGER,
	`Field3`	año de lanzamiento,
	`Field4`	costo de película,
	`Field5`	director de cine
);
INSERT INTO sqlitebrowser_rename_column_new_table SELECT `Field1`,`Field2`,`Field3`,`Field4`,`Field5` FROM `Película`;
PRAGMA defer_foreign_keys
PRAGMA defer_foreign_keys = "1";
DROP TABLE `Película`;
ALTER TABLE `sqlitebrowser_rename_column_new_table` RENAME TO `Película`
PRAGMA defer_foreign_keys = "0";
SELECT type,name,sql,tbl_name,'0' AS temp FROM sqlite_master UNION SELECT type,name,sql,tbl_name,'1' AS temp FROM sqlite_temp_master; 
