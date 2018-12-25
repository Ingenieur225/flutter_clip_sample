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

2.
<img src="section2.png" width="250"/>

    Path getClip(Size size) {
        final path = Path();
        path.lineTo(0.0, size.height);
        var firstPoint = Offset(size.width*0.5, size.height - 90);
        var firstEndPoint = Offset(size.width, size.height);
        path.quadraticBezierTo(firstPoint.dx, firstPoint.dy, firstEndPoint.dx, firstEndPoint.dy);
        path.lineTo(size.width, size.height);
        path.lineTo(size.width, 0.0);
        return path;
    }


3.
<img src="section3.png" width="250"/>

   Path getClip(Size size) {
        final path = Path();
        path.lineTo(0.0, size.height - 50);
        var firstPoint = Offset(size.width*0.5, size.height + 50);
        var firstEndPoint = Offset(size.width, size.height - 50);
        path.quadraticBezierTo(firstPoint.dx, firstPoint.dy, firstEndPoint.dx, firstEndPoint.dy);
        path.lineTo(size.width, size.height - 50 );
        path.lineTo(size.width, 0.0);
        return path;
  }
       
4.
<img src="section4.png" width="250"/>

    Path getClip(Size size) {
        final path = Path();
        path.lineTo(0.0, size.height - 60);
        path.lineTo(size.width*.35, size.height - 60);
        path.lineTo(size.width*.5, size.height);
        path.lineTo(size.width*.65, size.height - 60);
        path.lineTo(size.width, size.height - 60);
        path.lineTo(size.width, 0.0);
        return path;
    }
       