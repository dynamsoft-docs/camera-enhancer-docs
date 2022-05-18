
* Optimized the UI configuration feature of `DCECameraView`.
  * Added interfaces to accept a few types of graphic elements, e.g. rectangles, quadrilaterals, lines, texts. Other SDKs would take advantages of these interfaces to simplify the output on graphic views.
  * APIs are available for users to add user defined UI elements.
* Added a new UI view `DCEImageEditorView`
  * The quadrilateral elements displayed on the view can be selected and edited. When an element is selected, user can adjust the border of the quadrilateral to make the coordinates more accurate. The vertices of an element are displayed outstandingly and zoomed-in to support users to move the points accurately.
  * DCE outputs the coordinates of interactively adjusted vertices of border sides, which can be used by further processing of other SDKs.

