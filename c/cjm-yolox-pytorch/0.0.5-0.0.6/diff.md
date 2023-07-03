# Comparing `tmp/cjm-yolox-pytorch-0.0.5.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.5.tar", last modified: Sat Jul  1 23:42:52 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.6.tar", last modified: Mon Jul  3 18:21:27 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.5.tar` & `cjm-yolox-pytorch-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:42:52.412919 cjm-yolox-pytorch-0.0.5/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.5/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.5/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:42:52.412749 cjm-yolox-pytorch-0.0.5/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-01 23:25:02.000000 cjm-yolox-pytorch-0.0.5/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:42:52.409917 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    20895 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15405 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:42:52.412250 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       31 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1052 2023-07-01 23:42:12.000000 cjm-yolox-pytorch-0.0.5/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-01 23:42:52.412970 cjm-yolox-pytorch-0.0.5/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.5/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 18:21:27.085583 cjm-yolox-pytorch-0.0.6/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.6/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.6/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 18:21:27.085422 cjm-yolox-pytorch-0.0.6/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-03 18:20:50.000000 cjm-yolox-pytorch-0.0.6/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 18:21:27.083003 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-03 18:20:46.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-03 18:20:46.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    21293 2023-07-03 18:20:46.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-03 18:20:46.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15405 2023-07-03 18:20:46.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-03 18:20:46.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 18:21:27.085093 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 18:21:27.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-03 18:21:27.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-03 18:21:27.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-03 18:21:27.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       31 2023-07-03 18:21:27.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-03 18:21:27.000000 cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1052 2023-07-03 17:55:04.000000 cjm-yolox-pytorch-0.0.6/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-03 18:21:27.085632 cjm-yolox-pytorch-0.0.6/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.6/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.5/LICENSE` & `cjm-yolox-pytorch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.5/PKG-INFO` & `cjm-yolox-pytorch-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.5/README.md` & `cjm-yolox-pytorch-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/_modidx.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/loss.py`

 * *Files 16% similar despite different names*

```diff
@@ -95,45 +95,45 @@
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/bbox/samplers/sampling_result.py#L7)
 
     """
     def __init__(self, 
                  positive_indices:np.array, # Indices of the positive samples.
                  negative_indices:np.array, # Indices of the negative samples.
-                 bounding_boxes:np.array, # Array containing all bounding boxes.
-                 ground_truth_bounding_boxes:torch.Tensor, # Tensor containing all ground truth bounding boxes.
+                 bboxes:np.array, # Array containing all bounding boxes.
+                 ground_truth_bboxes:torch.Tensor, # Tensor containing all ground truth bounding boxes.
                  assignment_result, # Object that contains the ground truth indices and labels corresponding to each sample.
                  ground_truth_flags:np.array # Array indicating which samples are ground truth.
                 ):
         # Indices of positive and negative samples
         self.positive_indices = positive_indices
         self.negative_indices = negative_indices
 
         # Bounding boxes for positive and negative samples
-        self.positive_bounding_boxes = bounding_boxes[positive_indices]
-        self.negative_bounding_boxes = bounding_boxes[negative_indices]
+        self.positive_bboxes = bboxes[positive_indices]
+        self.negative_bboxes = bboxes[negative_indices]
         
         # Flag indicating if the positive samples are ground truth
         self.is_positive_ground_truth = ground_truth_flags[positive_indices]
 
         # Number of ground truths
-        self.number_of_ground_truths = ground_truth_bounding_boxes.shape[0]
+        self.number_of_ground_truths = ground_truth_bboxes.shape[0]
         
         # Indices of the assigned ground truths for positive samples
         self.positive_assigned_ground_truth_indices = assignment_result.ground_truth_box_indices[positive_indices] - 1
 
         # Check the consistency of ground truth bounding boxes and assigned indices
-        if ground_truth_bounding_boxes.numel() == 0:
+        if ground_truth_bboxes.numel() == 0:
             if self.positive_assigned_ground_truth_indices.numel() != 0:
                 raise ValueError('Mismatch between ground truth bounding boxes and positive assigned ground truth indices.')
-            self.positive_ground_truth_bounding_boxes = torch.empty_like(ground_truth_bounding_boxes).view(-1, 4)
+            self.positive_ground_truth_bboxes = torch.empty_like(ground_truth_bboxes).view(-1, 4)
         else:
-            if len(ground_truth_bounding_boxes.shape) < 2:
-                ground_truth_bounding_boxes = ground_truth_bounding_boxes.view(-1, 4)
-            self.positive_ground_truth_bounding_boxes = ground_truth_bounding_boxes[self.positive_assigned_ground_truth_indices, :]
+            if len(ground_truth_bboxes.shape) < 2:
+                ground_truth_bboxes = ground_truth_bboxes.view(-1, 4)
+            self.positive_ground_truth_bboxes = ground_truth_bboxes[self.positive_assigned_ground_truth_indices, :]
 
         # If labels are assigned, assign labels for positive samples. Otherwise, set it as None
         if assignment_result.category_labels is not None:
             self.positive_ground_truth_labels = assignment_result.category_labels[positive_indices]
         else:
             self.positive_ground_truth_labels = None
 
@@ -143,15 +143,15 @@
     YOLOXLoss class implements the loss function used in the YOLOX model. 
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/dense_heads/yolox_head.py#L321)
 
     #### Pseudocode
-    1. Receive class_scores, predicted_bounding_boxes, objectness_scores, ground_truth_bounding_boxes, and ground_truth_labels as input. These are all tensors.
+    1. Receive class_scores, predicted_bboxes, objectness_scores, ground_truth_bboxes, and ground_truth_labels as input. These are all tensors.
     2. Calculate the size of the feature maps from class scores.
     3. Create multi-level prior boxes using the feature map sizes.
     4. Reshape and flatten class predictions, bounding box predictions, and objectness scores. 
     5. Combine the class predictions, bounding box predictions, and objectness scores from different levels into one tensor respectively.
     6. Combine the prior boxes from different levels into one tensor and decode the bounding boxes using these prior boxes and bounding box predictions.
     7. For each image, calculate the targets for classification, bounding box, objectness, and optionally, L1 loss.
     8. Determine the total number of positive samples.
@@ -160,27 +160,37 @@
         - If L1 loss is enabled, calculate the L1 loss using the bounding box predictions and L1 targets.
     11. Return a dictionary containing the classification, bounding box, objectness, and optionally, L1 loss.
     
     
     """
     def __init__(self, 
                  num_classes:int, # The number of target classes.
-                 bounding_box_loss_func, # The loss function to calculate the bounding box regression loss.
-                 class_loss_func, # The loss function to calculate the classification loss.
-                 objectness_loss_func, # The loss function to calculate the objectness loss.
-                 l1_loss_func, # The loss function to calculate the L1 loss.
+                 bbox_loss_weight:float=2.0, # The weight for the loss function to calculate the bounding box regression loss.
+                 class_loss_weight:float=1.0, # The weight for the loss function to calculate the classification loss.
+                 objectness_loss_weight:float=1.0, # The weight for the loss function to calculate the objectness loss.
+                 l1_loss_weight:float=1.0, # The weight for the loss function to calculate the L1 loss.
                  use_l1:bool=False, # Whether to use L1 loss in the calculation.
                  strides:List[int]=[8,16,32] # The list of strides.
                 ):
         
         self.num_classes = num_classes
-        self.bounding_box_loss_func = bounding_box_loss_func
-        self.class_loss_func = class_loss_func
-        self.objectness_loss_func = objectness_loss_func
-        self.l1_loss_func = l1_loss_func
+        
+        giou_loss_partial = partial(torchvision.ops.generalized_box_iou_loss, reduction='none', eps=1e-16)
+        self.bbox_loss_func = lambda bx1, bx2 : (1-(1-giou_loss_partial(boxes1=bx1, boxes2=bx2))**2).sum()
+        self.class_loss_func = partial(F.binary_cross_entropy_with_logits, reduction='sum')
+        self.objectness_loss_func = partial(F.binary_cross_entropy_with_logits, reduction='sum')
+        self.l1_loss_func = partial(F.l1_loss, reduction='sum')
+        
+        
+        self.bbox_loss_weight = bbox_loss_weight
+        self.class_loss_weight = class_loss_weight
+        self.objectness_loss_weight = objectness_loss_weight
+        self.l1_loss_weight = l1_loss_weight
+        
+        
         self.use_l1 = use_l1
         
         # Initialize the prior box generator and assigner
         self.prior_generator = MlvlPointGenerator(strides, offset=0)
         self.assigner = SimOTAAssigner(center_radius=2.5)
         
     def bbox_decode(self, prior_boxes, predicted_boxes):
@@ -204,32 +214,32 @@
 
         # Stack coordinates to create decoded bounding boxes
         decoded_boxes = torch.cat((top_left, bottom_right), -1)
 
         return decoded_boxes
 
 
-    def sample(self, assignment_result, bounding_boxes, ground_truth_boxes, **kwargs):
+    def sample(self, assignment_result, bboxes, ground_truth_boxes, **kwargs):
         """
         Samples positive and negative indices based on the assignment result.
         
         Args:
             assignment_result (Object): The assignment result obtained from assigner.
-            bounding_boxes (torch.Tensor): The predicted bounding boxes.
+            bboxes (torch.Tensor): The predicted bounding boxes.
             ground_truth_boxes (torch.Tensor): The ground truth boxes.
 
         Returns:
             SamplingResult: The sampling result containing positive and negative indices.
         """
         positive_indices = torch.nonzero(
             assignment_result.ground_truth_box_indices > 0, as_tuple=False).squeeze(-1).unique()
         negative_indices = torch.nonzero(
             assignment_result.ground_truth_box_indices == 0, as_tuple=False).squeeze(-1).unique()
-        ground_truth_flags = bounding_boxes.new_zeros(bounding_boxes.shape[0], dtype=torch.uint8)
-        sampling_result = SamplingResult(positive_indices, negative_indices, bounding_boxes, ground_truth_boxes,
+        ground_truth_flags = bboxes.new_zeros(bboxes.shape[0], dtype=torch.uint8)
+        sampling_result = SamplingResult(positive_indices, negative_indices, bboxes, ground_truth_boxes,
                                          assignment_result, ground_truth_flags)
         return sampling_result
 
 
     def get_l1_target(self, l1_target, ground_truth_boxes, prior_boxes, epsilon=1e-8):
         """
         Calculates the L1 target.
@@ -245,59 +255,59 @@
         """
         ground_truth_centroid_and_wh = torchvision.ops.box_convert(ground_truth_boxes, 'xyxy', 'cxcywh')
         l1_target[:, :2] = (ground_truth_centroid_and_wh[:, :2] - prior_boxes[:, :2]) / prior_boxes[:, 2:]
         l1_target[:, 2:] = torch.log(ground_truth_centroid_and_wh[:, 2:] / prior_boxes[:, 2:] + epsilon)
         return l1_target
 
 
-    def get_target_single(self, class_preds, objectness_score, prior_boxes, decoded_bounding_boxes,
-                           ground_truth_bounding_boxes, ground_truth_labels):
+    def get_target_single(self, class_preds, objectness_score, prior_boxes, decoded_bboxes,
+                           ground_truth_bboxes, ground_truth_labels):
         """
         Calculates the targets for a single image.
 
         Args:
             class_preds (torch.Tensor): The predicted class probabilities.
             objectness_score (torch.Tensor): The predicted objectness scores.
             prior_boxes (torch.Tensor): The prior bounding boxes.
-            decoded_bounding_boxes (torch.Tensor): The decoded bounding boxes.
-            ground_truth_bounding_boxes (torch.Tensor): The ground truth boxes.
+            decoded_bboxes (torch.Tensor): The decoded bounding boxes.
+            ground_truth_bboxes (torch.Tensor): The ground truth boxes.
             ground_truth_labels (torch.Tensor): The ground truth labels.
 
         Returns:
             Tuple: The targets for classification, objectness, bounding boxes, and L1 (if applicable), along with
             the foreground mask and the number of positive samples.
         """
         # Get the number of prior boxes and ground truth labels
         num_prior_boxes = prior_boxes.size(0)
         num_ground_truths = ground_truth_labels.size(0)
 
         # Match dtype of ground truth bounding boxes to the dtype of decoded bounding boxes
-        ground_truth_bounding_boxes = ground_truth_bounding_boxes.to(decoded_bounding_boxes.dtype)
+        ground_truth_bboxes = ground_truth_bboxes.to(decoded_bboxes.dtype)
 
         # Check if there are no ground truth labels (objects) in the image
         if num_ground_truths == 0:
             # Initialize targets as zero tensors, and foreground_mask as a boolean tensor with False values
             class_targets = class_preds.new_zeros((0, self.num_classes))
-            bounding_box_targets = class_preds.new_zeros((0, 4))
+            bbox_targets = class_preds.new_zeros((0, 4))
             l1_targets = class_preds.new_zeros((0, 4))
             objectness_targets = class_preds.new_zeros((num_prior_boxes, 1))
             foreground_mask = class_preds.new_zeros(num_prior_boxes).bool()
-            return (foreground_mask, class_targets, objectness_targets, bounding_box_targets,
+            return (foreground_mask, class_targets, objectness_targets, bbox_targets,
                     l1_targets, 0)  # Return zero for num_positive_per_image
 
         # Calculate the offset for the prior boxes
         offset_prior_boxes = torch.cat([prior_boxes[:, :2] + prior_boxes[:, 2:] * 0.5, prior_boxes[:, 2:]], dim=-1)
 
         # Assign ground truth objects to prior boxes and get assignment results
         assignment_result = self.assigner.assign(
             class_preds.sigmoid() * objectness_score.unsqueeze(1).sigmoid(),
-            offset_prior_boxes, decoded_bounding_boxes, ground_truth_bounding_boxes, ground_truth_labels)
+            offset_prior_boxes, decoded_bboxes, ground_truth_bboxes, ground_truth_labels)
 
         # Use assignment results to sample prior boxes
-        sampling_result = self.sample(assignment_result, prior_boxes, ground_truth_bounding_boxes)
+        sampling_result = self.sample(assignment_result, prior_boxes, ground_truth_bboxes)
         
         # Get the indices of positive (object-containing) samples
         positive_indices = sampling_result.positive_indices
         num_positive_per_image = positive_indices.size(0)
 
         # Get the maximum IoU values for the positive samples
         positive_ious = assignment_result.max_iou_values[positive_indices]
@@ -306,107 +316,114 @@
         class_targets = F.one_hot(sampling_result.positive_ground_truth_labels, self.num_classes) * positive_ious.unsqueeze(-1)
 
         # Initialize objectness targets as zeros and set the values at positive_indices to 1
         objectness_targets = torch.zeros_like(objectness_score).unsqueeze(-1)
         objectness_targets[positive_indices] = 1
 
         # Generate bounding box targets
-        bounding_box_targets = sampling_result.positive_ground_truth_bounding_boxes
+        bbox_targets = sampling_result.positive_ground_truth_bboxes
 
         # Initialize L1 targets as zeros
         l1_targets = class_preds.new_zeros((num_positive_per_image, 4))
 
         # If use_l1 is True, calculate L1 targets
         if self.use_l1:
-            l1_targets = self.get_l1_target(l1_targets, bounding_box_targets, prior_boxes[positive_indices])
+            l1_targets = self.get_l1_target(l1_targets, bbox_targets, prior_boxes[positive_indices])
 
         # Initialize foreground_mask as zeros and set the values at positive_indices to True
         foreground_mask = torch.zeros_like(objectness_score).to(torch.bool)
         foreground_mask[positive_indices] = 1
 
         # Return the computed targets, the foreground mask, and the number of positive samples per image
-        return (foreground_mask, class_targets, objectness_targets, bounding_box_targets, l1_targets, num_positive_per_image)
+        return (foreground_mask, class_targets, objectness_targets, bbox_targets, l1_targets, num_positive_per_image)
     
     
     def flatten_and_concat(self, tensors, num_images, reshape_dims=None):
         new_shape = (num_images, -1, reshape_dims) if reshape_dims else (num_images, -1)
         return torch.cat([t.permute(0, 2, 3, 1).reshape(*new_shape) for t in tensors], dim=1)
 
     
-    def __call__(self, num_images, class_scores, predicted_bounding_boxes, objectness_scores, ground_truth_bounding_boxes, ground_truth_labels):
+    def __call__(self, num_images, class_scores, predicted_bboxes, objectness_scores, ground_truth_bboxes, ground_truth_labels):
         """
         Main method to compute the YOLOX loss.
 
         Args:
             num_images (int): The number of images in a batch.
             class_scores (List[torch.Tensor]): A list of class scores for each scale.
-            predicted_bounding_boxes (List[torch.Tensor]): A list of predicted bounding boxes for each scale.
+            predicted_bboxes (List[torch.Tensor]): A list of predicted bounding boxes for each scale.
             objectness_scores (List[torch.Tensor]): A list of objectness scores for each scale.
-            ground_truth_bounding_boxes (List[torch.Tensor]): A list of ground truth bounding boxes for each image.
+            ground_truth_bboxes (List[torch.Tensor]): A list of ground truth bounding boxes for each image.
             ground_truth_labels (List[torch.Tensor]): A list of ground truth labels for each image.
 
         Returns:
             Dict: A dictionary with the classification, bounding box, objectness, and optionally, L1 loss.
         """
         # Compute feature map sizes from class scores
         feature_map_sizes = [class_score.shape[2:] for class_score in class_scores]
 
         # Generate multi-level priors
         multilevel_prior_boxes = self.prior_generator.grid_priors(
             feature_map_sizes, class_scores[0].device, with_stride=True)
         
         # Flatten and concatenate class predictions, bounding box predictions, and objectness scores
         flatten_class_preds = self.flatten_and_concat(class_scores, num_images, self.num_classes)
-        flatten_bounding_box_preds = self.flatten_and_concat(predicted_bounding_boxes, num_images, 4)
+        flatten_bbox_preds = self.flatten_and_concat(predicted_bboxes, num_images, 4)
         flatten_objectness_scores = self.flatten_and_concat(objectness_scores, num_images)
                     
         # Concatenate and decode prior boxes
         flatten_prior_boxes = torch.cat(multilevel_prior_boxes)
-        flatten_decoded_bounding_boxes = self.bbox_decode(flatten_prior_boxes, flatten_bounding_box_preds)
+        flatten_decoded_bboxes = self.bbox_decode(flatten_prior_boxes, flatten_bbox_preds)
 
         # Compute targets
-        (positive_masks, class_targets, objectness_targets, bounding_box_targets, l1_targets,
+        (positive_masks, class_targets, objectness_targets, bbox_targets, l1_targets,
          num_positive_images) = multi_apply(
              self.get_target_single, flatten_class_preds.detach(),
              flatten_objectness_scores.detach(),
              flatten_prior_boxes.unsqueeze(0).repeat(num_images, 1, 1),
-             flatten_decoded_bounding_boxes.detach(), ground_truth_bounding_boxes, ground_truth_labels)
+             flatten_decoded_bboxes.detach(), ground_truth_bboxes, ground_truth_labels)
 
         # Calculate total number of samples
         num_total_samples = max(sum(num_positive_images), 1)
 
         # Concatenate all positive masks, class targets, objectness targets, and bounding box targets
         positive_masks = torch.cat(positive_masks, 0)
         class_targets = torch.cat(class_targets, 0)
         objectness_targets = torch.cat(objectness_targets, 0)
-        bounding_box_targets = torch.cat(bounding_box_targets, 0)
+        bbox_targets = torch.cat(bbox_targets, 0)
 
         # If use_l1 is True, concatenate l1 targets
         if self.use_l1:
             l1_targets = torch.cat(l1_targets, 0)
 
         # Compute bounding box loss
-        loss_bbox = self.bounding_box_loss_func(
-            flatten_decoded_bounding_boxes.view(-1, 4)[positive_masks],
-            bounding_box_targets) / num_total_samples
+        loss_bbox = self.bbox_loss_func(
+            flatten_decoded_bboxes.view(-1, 4)[positive_masks],
+            bbox_targets) / num_total_samples
 
         # Compute objectness loss
         loss_obj = self.objectness_loss_func(flatten_objectness_scores.view(-1, 1),
                                  objectness_targets) / num_total_samples
 
         # Compute class loss
         loss_cls = self.class_loss_func(
             flatten_class_preds.view(-1, self.num_classes)[positive_masks],
             class_targets) / num_total_samples
+                
+        # Scale losses
+        loss_bbox *= self.bbox_loss_weight
+        loss_obj *= self.objectness_loss_weight
+        loss_cls *= self.class_loss_weight
+        
 
         # Initialize loss dictionary
         loss_dict = dict(loss_cls=loss_cls, loss_bbox=loss_bbox, loss_obj=loss_obj)
 
         # If use_l1 is True, compute L1 loss and add it to the loss dictionary
         if self.use_l1:
             loss_l1 = self.l1_loss_func(
-                flatten_bounding_box_preds.view(-1, 4)[positive_masks],
+                flatten_bbox_preds.view(-1, 4)[positive_masks],
                 l1_targets) / num_total_samples
+            loss_l1 *= self.l1_loss_weight
             loss_dict.update(loss_l1=loss_l1)
 
         # Return loss dictionary
         return loss_dict
```

### Comparing `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/simota.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.6/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.5/settings.ini` & `cjm-yolox-pytorch-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
```

### Comparing `cjm-yolox-pytorch-0.0.5/setup.py` & `cjm-yolox-pytorch-0.0.6/setup.py`

 * *Files identical despite different names*

