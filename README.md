# Clipper code by Dart

1. 
<img src="section1.png" width="250"/>

      Path getClip(Size size) {
            final path = Path();
            path.lineTo(0.0, size.height);
            var firstPoint = Offset(size.width*0.25, size.height - 60);
            var firstEndPoint = Offset(size.width*0.5, size.height);
            path.quadraticBezierTo(firstPoint.dx, firstPoint.dy, firstEndPoint.dx, firstEndPoint.dy);
            var sencondPoint = Offset(size.width*0.75, size.height - 60);
            var sencondEndPoint = Offset(size.width, size.height);
            path.quadraticBezierTo(sencondPoint.dx, sencondPoint.dy, sencondEndPoint.dx, sencondEndPoint.dy);
            path.lineTo(size.width, size.height);
            path.lineTo(size.width, 0.0);
            return path;
      }





       
