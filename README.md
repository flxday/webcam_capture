# webcam_capture
Just webcam capture and playing using OpenCV

ORB

Class that implements a descriptor for key points. It uses an algorithm for Detecion selecionar key points and features


//ORB point feature detector 
cv::Ptr<cv::ORB> orb_detector = new cv::ORB(10); 
FeatureDetector::create 
C++: Ptr<FeatureDetector> FeatureDetector::create(const string& detectorType) 


//set of point features 
cv::vector<cv::KeyPoint> point_set; 
//FeatureDetector::detect 
//C++: void FeatureDetector::detect(const Mat& image, vector<KeyPoint>& keypoints, const Mat& mask=Mat() ) const 



//ORB descriptor 
cv::Ptr<cv::DescriptorExtractor> orb_descriptor; 
clase descriptorExtractor. 
//class to define descriptors for calculating key points of the image.
 


//init the descriptor 
orb_descriptor = cv::DescriptorExtractor::create("ORB"); 
//ORB initiation descriptor



//set of descriptors, for each feature there is an associated descriptor
cv::Mat descriptor_set; 
Mat constant allocation to a set of descriptors.

http://docs.opencv.org/2.4/modules/features2d/doc/feature_detection_and_description.html
