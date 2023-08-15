import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';

class sensorCard extends StatefulWidget {
  sensorCard({super.key, required this.temp, required this.sensorType, required this.unit});
  final double temp;
  final String sensorType;
  final String unit;

  @override
  State<sensorCard> createState() => _sensorCardState();
}

class _sensorCardState extends State<sensorCard> {
  @override
  Widget build(BuildContext context) {
    // TODO: implement build
    return Container(
      margin: EdgeInsets.fromLTRB(10, 15, 5, 15),
      width: 100,
      height: 70,
      decoration: const BoxDecoration(
          borderRadius: BorderRadius.only(
            bottomLeft: Radius.circular(7),
            bottomRight: Radius.circular(7),
            topLeft: Radius.circular(7),
            topRight: Radius.circular(7),
          ),
          color: Colors.white),
      child: Container(
        width: 100,
        child: Stack(
          children: [
            Positioned(
              bottom: 10,
              child: SizedBox(
                width: 100,
                child: Text(
                  widget.sensorType,
                  style: GoogleFonts.plusJakartaSans(
                    fontSize: 13,
                    fontWeight: FontWeight.bold,
                    fontStyle: FontStyle.normal,
                  ),
                  textAlign: TextAlign.center,
                ),
              ),
            ),
            Positioned(
              top: 5,
              right: 10,
              child: Text(
                widget.temp.toString(),
                style: GoogleFonts.plusJakartaSans(
                  fontSize: 18,
                  fontWeight: FontWeight.bold,
                  fontStyle: FontStyle.normal,
                ),
                textAlign: TextAlign.center,
              ),
            ),
            Positioned(
              top: 25,
              right: 10,
              child: Text(
                widget.unit,
                style: GoogleFonts.plusJakartaSans(
                  fontSize: 10,
                  fontWeight: FontWeight.bold,
                  fontStyle: FontStyle.normal,
                ),
                textAlign: TextAlign.center,
              ),
            ),
          ],
        ),
      ),
    );
  }
}
