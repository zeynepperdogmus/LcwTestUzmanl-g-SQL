# LcwTestUzmanl-g-SQL


CREATE TABLE employee (
    id INTEGER PRIMARY KEY,
    name VARCHAR(50),
    birthday DATE,
    email VARCHAR(100)
);

INSERT INTO employee (id, name, birthday, email)
VALUES
(1, 'Ahmet Yılmaz', '1990-05-15', 'ahmet.yilmaz@example.com'),
(2, 'Mehmet Demir', '1985-03-22', 'mehmet.demir@example.com'),
(3, 'Ayşe Kaya', '1992-07-30', 'ayse.kaya@example.com'),
(4, 'Fatma Çelik', '1988-11-04', 'fatma.celik@example.com'),
(5, 'Ali Arslan', '1995-02-18', 'ali.arslan@example.com'),
(6, 'Veli Özdemir', '1990-09-25', 'veli.ozdemir@example.com'),
(7, 'Emine Şahin', '1982-01-30', 'emine.sahin@example.com'),
(8, 'Mustafa Korkmaz', '1987-12-10', 'mustafa.korkmaz@example.com'),
(9, 'Zeynep Aydın', '1994-06-15', 'zeynep.aydin@example.com'),
(10, 'İbrahim Demirtaş', '1983-04-23', 'ibrahim.demirtas@example.com'),
(11, 'Cemre Gürbüz', '1996-03-14', 'cemre.gurbuz@example.com'),
(12, 'Kemal Aslan', '1991-07-02', 'kemal.aslan@example.com'),
(13, 'Seda Yıldız', '1989-08-19', 'seda.yildiz@example.com'),
(14, 'Hakan Özkan', '1993-01-11', 'hakan.ozkan@example.com'),
(15, 'Gülcan Yılmaz', '1986-12-05', 'gulcan.yilmaz@example.com'),
(16, 'Orhan Güler', '1990-10-14', 'orhan.guler@example.com'),
(17, 'Serap Çetin', '1984-07-21', 'serap.cetin@example.com'),
(18, 'Nihat Türkmen', '1992-04-02', 'nihat.turkmen@example.com'),
(19, 'Duygu Şimşek', '1994-11-30', 'duygu.simsek@example.com'),
(20, 'Cengiz Erdem', '1987-03-13', 'cengiz.erdem@example.com'),
(21, 'Sibel Kılıç', '1995-05-09', 'sibel.kilic@example.com'),
(22, 'Fikret Akbulut', '1990-08-17', 'fikret.akbulut@example.com'),
(23, 'Aylin Koç', '1989-12-22', 'aylin.koc@example.com'),
(24, 'Barış Yavuz', '1993-01-01', 'baris.yavuz@example.com'),
(25, 'Canan Çetin', '1991-06-13', 'canan.cetin@example.com'),
(26, 'Serdar Atalay', '1982-10-30', 'serdar.atalay@example.com'),
(27, 'Merve Sönmez', '1988-02-16', 'merve.sonmez@example.com'),
(28, 'Recep Akın', '1994-07-05', 'recep.akin@example.com'),
(29, 'Büşra Kaya', '1986-09-17', 'busra.kaya@example.com'),
(30, 'Yusuf Uçar', '1992-11-01', 'yusuf.ucar@example.com'),
(31, 'Tuba Acar', '1995-04-23', 'tuba.acar@example.com'),
(32, 'Gökhan İnal', '1984-06-30', 'gokhan.inal@example.com'),
(33, 'Seda Tok', '1990-05-28', 'seda.tok@example.com'),
(34, 'Onur Tuncer', '1993-02-02', 'onur.tuncer@example.com'),
(35, 'Nurgül Kara', '1987-12-01', 'nurgul.kara@example.com'),
(36, 'Feryal Aydoğdu', '1996-08-24', 'feryal.aydogdu@example.com'),
(37, 'Murat Sarı', '1990-03-09', 'murat.sari@example.com'),
(38, 'Şule Koçak', '1983-05-17', 'sule.kocak@example.com'),
(39, 'Halil Yalçın', '1991-01-13', 'halil.yalcin@example.com'),
(40, 'Melis Baran', '1992-09-15', 'melis.baran@example.com'),
(41, 'Özlem Erdem', '1985-10-04', 'ozlem.erdem@example.com'),
(42, 'Aliye Bilgin', '1993-04-14', 'aliye.bilgin@example.com'),
(43, 'Berkay Çakır', '1994-10-11', 'berkay.cakir@example.com'),
(44, 'Zeynep Alkan', '1988-03-01', 'zeynep.alkan@example.com'),
(45, 'Emir Aktaş', '1991-05-13', 'emir.aktas@example.com'),
(46, 'Nisa Kaplan', '1995-08-08', 'nisa.kaplan@example.com'),
(47, 'Yusuf Akbaş', '1982-02-10', 'yusuf.akbas@example.com'),
(48, 'Murat Çetin', '1989-07-26', 'murat.cetin@example.com'),
(49, 'Ayşe Avcı', '1994-10-04', 'ayse.avci@example.com'),
(50, 'Fatma Yılmaz', '1990-06-17', 'fatma.yilmaz@example.com');



-- id'ye göre güncelleme
UPDATE employee SET name = 'Emine Güler' WHERE id = 1;

-- name'e göre güncelleme
UPDATE employee SET email = 'ahmet.yilmaz@newemail.com' WHERE name = 'Ahmet Yılmaz';

-- birthday'e göre güncelleme
UPDATE employee SET birthday = '1985-11-11' WHERE birthday = '1992-07-30';

-- email'e göre güncelleme
UPDATE employee SET name = 'Mustafa Demir' WHERE email = 'mehmet.demir@example.com';

-- id'ye göre güncelleme
UPDATE employee SET email = 'seda.yildiz@newmail.com' WHERE id = 2;




-- id'ye göre silme
DELETE FROM employee WHERE id = 1;

-- name'e göre silme
DELETE FROM employee WHERE name = 'Mehmet Demir';

-- birthday'e göre silme
DELETE FROM employee WHERE birthday = '1988-11-04';

-- email'e göre silme
DELETE FROM employee WHERE email = 'ali.arslan@example.com';

-- id'ye göre silme
DELETE FROM employee WHERE id = 3;




