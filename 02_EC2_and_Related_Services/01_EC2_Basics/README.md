# EC2 Basics

This section covers fundamental EC2 concepts and operations that are essential for SysOps administrators. Each topic includes both theoretical understanding and practical hands-on exercises.

## Content Structure

### 1. Instance Management
- **1.1Changing EC2 Instance Type** (4 minutes)
  - **Lý do thay đổi loại phiên bản**:
    - Nâng cấp từ t2.micro lên t2.small để có thêm RAM và CPU
    - Tối ưu hóa hiệu suất ứng dụng
    - Đáp ứng nhu cầu tăng trưởng của ứng dụng
  
  - **Điều kiện thay đổi**:
    - Phiên bản phải sử dụng EBS (Elastic Block Store)
    - Phiên bản phải ở trạng thái dừng (stopped)
    - Có đủ quyền để thay đổi thuộc tính instance

  - **Quy trình thực hiện**:
    1. Dừng phiên bản EC2
    2. Thay đổi loại phiên bản thông qua:
       - Click chuột phải vào instance
       - Chọn "Change Instance Type"
       - Chọn loại phiên bản mới (ví dụ: t2.small)
    3. Khởi động lại phiên bản

  - **Lưu ý quan trọng**:
    - Một số loại phiên bản hỗ trợ EBS-optimized
    - Khi dừng và khởi động lại, instance có thể chạy trên máy chủ vật lý khác
    - Dữ liệu được bảo toàn vì sử dụng EBS
    - Địa chỉ IP có thể thay đổi nếu không sử dụng Elastic IP

  - **Kết quả thay đổi**:
    - Tăng RAM (ví dụ: từ 993 MB lên 1,991 MB)
    - Cải thiện hiệu suất ứng dụng
    - Có thể quay lại phiên bản miễn phí (t2.micro) nếu cần



- **EC2 Hibernate Hands On** (4 minutes)
  - Practical implementation
  - Configuration steps
  - Testing hibernation

### 2. Networking
- **Enhanced Networking** (4 minutes)
  - Network performance optimization
  - ENI configuration
  - Best practices

- **Elastic IPs** (6 minutes)
  - EIP concepts and usage
  - Association and disassociation
  - Cost considerations

- **IP Address Charges in AWS** (6 minutes)
  - Understanding IP pricing
  - Cost optimization strategies
  - Best practices

### 3. Instance Placement
- **EC2 Placement Groups** (6 minutes)
  - Types of placement groups
  - Use cases and benefits
  - Configuration options

- **EC2 Placement Groups - Hands On** (2 minutes)
  - Practical implementation
  - Group creation and management
  - Instance placement

### 4. Instance Purchasing Options
- **EC2 Instance Purchasing Options** (10 minutes)
  - On-Demand instances
  - Reserved instances
  - Dedicated hosts
  - Cost comparison

- **Spot Instances & Spot Fleet** (10 minutes)
  - Spot instance concepts
  - Spot fleet configuration
  - Best practices and use cases

- **EC2 Instances Launch Types Hands On** (9 minutes)
  - Practical implementation
  - Configuration steps
  - Testing different launch types

- **Burstable Instances** (6 minutes)
  - T2/T3 instance concepts
  - CPU credits
  - Performance optimization

### 5. Monitoring and Troubleshooting
- **CloudWatch Metrics for EC2** (5 minutes)
  - Key metrics to monitor
  - Metric interpretation
  - Alert configuration

- **Unified CloudWatch Agent - Overview** (3 minutes)
  - Agent capabilities
  - Installation options
  - Configuration basics

- **Unified CloudWatch Agent - Hands On** (17 minutes)
  - Installation and configuration
  - Metric collection
  - Log management

- **EC2 Instance Status Checks** (5 minutes)
  - System and instance checks
  - Status interpretation
  - Troubleshooting steps

- **EC2 Instance Status Checks Hands On** (6 minutes)
  - Practical implementation
  - Check configuration
  - Status monitoring

- **EC2 Instance Status Checks - MUST KNOW** (1 minute)
  - Critical checks
  - Quick reference guide
  - Best practices

### 6. Troubleshooting
- **Troubleshooting EC2 Launch Issues** (4 minutes)
  - Common launch problems
  - Diagnostic steps
  - Resolution methods

- **Troubleshooting EC2 SSH Issues** (7 minutes)
  - SSH connection problems
  - Security group configuration
  - Key pair management

### 7. Cleanup and Assessment
- **EC2 Cleanup** (1 minute)
  - Resource cleanup procedures
  - Cost optimization
  - Best practices

- **Quiz: EC2 For SysOps Quiz**
  - Assessment of knowledge
  - Practical scenarios
  - Best practices review

## Learning Objectives

By the end of this section, you will be able to:
- Manage EC2 instances effectively
- Configure and optimize EC2 networking
- Implement proper monitoring and logging
- Troubleshoot common EC2 issues
- Optimize EC2 costs and performance
- Follow AWS best practices for EC2 management

## Prerequisites

- Basic understanding of AWS services
- Familiarity with Linux/Windows system administration
- Knowledge of networking concepts
- Understanding of cloud computing fundamentals 