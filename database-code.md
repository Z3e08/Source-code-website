-- phpMyAdmin SQL Dump
-- version 5.1.1
-- https://www.phpmyadmin.net/
--
-- Host: 127.0.0.1:3306
-- Generation Time: Dec 14, 2021 at 07:49 PM
-- Server version: 5.7.36
-- PHP Version: 7.4.26

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Database: `streetwear`
--

-- --------------------------------------------------------

--
-- Table structure for table `brands`
--

DROP TABLE IF EXISTS `brands`;
CREATE TABLE IF NOT EXISTS `brands` (
  `id` int(4) NOT NULL AUTO_INCREMENT,
  `Brand name` varchar(128) CHARACTER SET hp8 NOT NULL,
  `Location` varchar(1000) CHARACTER SET hp8 NOT NULL,
  `date` datetime NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=MyISAM AUTO_INCREMENT=5 DEFAULT CHARSET=latin1;

--
-- Dumping data for table `brands`
--

INSERT INTO `brands` (`id`, `Brand name`, `Location`, `date`) VALUES
(1, 'Supreme', 'United States New York', '1994-04-25 11:30:02'),
(2, 'Bape', 'Japan', '1996-06-12 10:31:14'),
(3, 'Off-White', 'Italy Milan', '2012-08-12 18:32:35'),
(4, 'MCM', 'Munich, Germany', '1976-04-15 11:10:01');

-- --------------------------------------------------------

--
-- Table structure for table `item`
--

DROP TABLE IF EXISTS `item`;
CREATE TABLE IF NOT EXISTS `item` (
  `ID` int(11) NOT NULL AUTO_INCREMENT,
  `Item Name` text NOT NULL,
  `Release Date` text NOT NULL,
  `Price` int(10) NOT NULL,
  PRIMARY KEY (`ID`)
) ENGINE=MyISAM AUTO_INCREMENT=31 DEFAULT CHARSET=latin1;

--
-- Dumping data for table `item`
--

INSERT INTO `item` (`ID`, `Item Name`, `Release Date`, `Price`) VALUES
(1, 'Supreme Tiffany & Co. Box Logo Tee', 'FW21', 54),
(2, 'Supreme Berlin Box Logo Tee', 'FW21', 48),
(3, 'Supreme Box Logo L/S Tee', 'FW20', 48),
(4, 'Supreme Emilio Pucci Box Logo Tee', 'SS21', 54),
(5, 'Supreme Box Logo Crewneck', 'FW18', 158),
(6, 'Bape adidas Superstar', '05/01/2021', 150),
(7, 'BAPE Premium Happy New Year 2021 Mens Backpack', 'FW20', 599),
(8, 'BAPE Color Camo Logo Full Zip Hoodie', 'SS20', 375),
(9, 'Bape x Uno Mattel Creations Cards', 'FW21', 26),
(10, 'BAPE 1st Camo Shark Full Zip Hoodie', 'FW18', 435),
(11, 'BAPE x MCM Camo Slide Sandals', 'FW19', 355),
(12, 'BAPE x MCM Rhinestone College Tee', 'FW19', 195),
(13, 'MCM Claus M Reversible Belt', '', 295),
(14, 'MCM Visetos Print T-shirt', '', 295),
(15, 'MCM Classic Logo T-shirt', '', 245),
(16, 'Off-White x Jordan T-shirt', 'FW21', 100),
(17, 'Nike Air Zoom Tempo NEXT%', '07/23/2021', 260),
(18, 'Jordan 2 Retro Low SP', '11/12/2021', 250),
(19, 'Converse Chuck Taylor All-Star', '10/08/2018', 130),
(20, 'Off-White Industrial Belt', 'SS19', 225);
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
