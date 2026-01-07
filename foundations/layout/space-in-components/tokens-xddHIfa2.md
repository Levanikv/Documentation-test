
# Tokens

---

# Static

Static tokens define fixed spacing values that remain the same across all screen sizes. They provide a solid foundation for spacing within components, ensuring consistent visual structure regardless of device.

**Characteristics:**

- **Fixed values:** Same pixel measurements at every breakpoint

- **Predictable behavior**: No variation during responsive change

  
**Inset**  
The `wel.sem.spacingStatic.inset` tokens define consistent spacing values for internal padding within components. These tokens provide a standardized scale for component padding that remains consistent across all breakpoints.  
  
**Token Group Space / wel / sem / spacingStatic / inset**:    
3xs: 2px  
2xs: 4px  
xs: 6px  
sm: 8px  
md: 16px  
lg: 20px  
xl: 24px  
2xl: 32px  
  
  
**Inline**  
The `wel.sem.spacingStatic.inline` tokens define horizontal spacing values for inline elements and layouts. These tokens provide a consistent scale for spacing between elements that sit side&hyphen;by&hyphen;side, such as Button, Badge, Chip, icons next to text, or items in a horizontal navigation.  
  
**Token Group Space / wel / sem / spacingStatic / inline**:    
3xs: 2px  
2xs: 4px  
xs: 8px  
sm: 12px  
md: 16px  
lg: 24px  
xl: 32px  
2xl: 40px  
3xl: 48px  
4xl: 56px  
5xl: 64px  
  
  
**Stack**  
The `wel.sem.spacingStatic.stack` tokens define vertical spacing values for inline elements and layouts. These tokens provide a consistent scale for spacing between elements that sit side&hyphen;by&hyphen;side, such as lists, inputs, slider, ...  
  
**Token Group Space / wel / sem / spacingStatic / stack**:    
3xs: 2px  
2xs: 4px  
xs: 8px  
sm: 12px  
md: 16px  
lg: 24px  
xl: 32px  
2xl: 40px  
  
  
**InsetSquish**  
The `wel.sem.spacingStatic.insetSquish` tokens provide asymmetric padding values where horizontal padding is greater than vertical padding, creating a "squished" appearance. These tokens are defined as pairs of horizontal (&hyphen;h) and vertical (&hyphen;v) values for consistent component padding across the design system.  
  
**Token Group Space / wel / sem / spacingStatic / insetSquish**:    
xs-h: 8px  
xs-v: 4px  
sm-h: 12px  
sm-v: 8px  
sm-h: 16px  
sm-v: 8px  
md-h: 16px  
md-v: 12px  
lg-h: 20px  
lg-v: 16px  
xl-h: 24px  
xl-v: 16px  
  
  
**InsetStretch**  
The `wel.sem.spacingStatic.insetStretch` tokens provide asymmetric padding values where vertical padding is greater than vertical padding, creating a "stretched" appearance. These tokens are defined as pairs of horizontal (&hyphen;h) and vertical (&hyphen;v) values for consistent component padding across the design system.  
  
**Token Group Space / wel / sem / spacingStatic / insetStretch**:    
sm-h: 12px  
sm-v: 16px  
md-h: 16px  
md-v: 24px  
lg-h: 16px  
lg-v: 32px  
xl-h: 24px  
xl-v: 32px  
  
  
**PinchHorizontal**  
The `wel.sem.spacingStatic.pinchHorizontal` tokens provide padding values only on the horizontal axis, creating a "pinched" appearance.  
  
**Token Group Space / wel / sem / spacingStatic / pinchHorizontal**:    
2xs: 4px  
xs: 8px  
sm: 12px  
md: 16px  
lg: 20px  
xl: 24px  
2xl: 32px  
  
  
**PinchVertical**  
The `wel.sem.spacingStatic.pinchVertical` tokens provide padding values only on the vertical axis, creating a "pinched" appearance.  
  
**Token Group Space / wel / sem / spacingStatic / pinchVertical**:    
2xs: 4px  
xs: 8px  
sm: 12px  
md: 16px  
lg: 24px  
xl: 32px  
2xl: 40px  
  


# Dynamic

Dynamic tokens provide responsive spacing values that adjust automatically based on screen size. They ensure layouts adapt fluidly to different devices while maintaining proper visual hierarchy.

**Characteristics:**

- **Responsive values:** Vary according to breakpoints

- **Screen&hyphen;aware:** Helps preserve visual balance across devices

  
**Inset**  
The `wel.sem.spacingDynamic.inset` tokens  provide responsive spacing values for homogeneous padding elements.  
D**ektop modes (medium and small).**  
  
**Token Group Space / wel / sem / spacingDynamic / inset**:    
xl: 24px  
2xl: 32px  
3xl: 48px  
4xl: 48px  
5xl: 64px  
  
**Tablet and mobile modes**.  
  
**Token Group Space / wel / sem / spacingDynamic / inset**:    
xl: 24px  
2xl: 32px  
3xl: 48px  
4xl: 48px  
5xl: 64px  
  
  
  
**Inline**  
The `wel.sem.spacingDynamic.inline`  provide responsive spacing values for inline elements in organisms, such as [Card](#), [Booking Engine](#), Carousel, ...  
  
**Dektop modes (medium and small).**  
  
**Token Group Space / wel / sem / spacingDynamic / inline**:    
xl: 24px  
3xl: 64px  
4xl: 64px  
6xl: 96px  
  
**Tablet and Mobile modes**  
  
**Token Group Space / wel / sem / spacingDynamic / inline**:    
xl: 24px  
3xl: 64px  
4xl: 64px  
6xl: 96px  
  
  
**Stack**  
The `wel.sem.spacingDynamic.stack` space tokens provide responsive spacing values for vertical aligned element.  
D**ektop modes (medium and small).**  
  
**Token Group Space / wel / sem / spacingDynamic / stack**:    
md: 16px  
lg: 24px  
xl: 32px  
2xl: 40px  
3xl: 48px  
4xl: 64px  
5xl: 96px  
  
**Tablet and Mobile modes**  
  
**Token Group Space / wel / sem / spacingDynamic / stack**:    
md: 16px  
lg: 24px  
xl: 32px  
2xl: 40px  
3xl: 48px  
4xl: 64px  
5xl: 96px  
  
  
**InsetSquish**  
The `wel.sem.spacingDynamic.insetSquish` tokens provide responsive spacing values for non homogeneous padding elements &hyphen; resulting in a visually squished layout. These tokens are defined as pairs of horizontal (&hyphen;h) and vertical (&hyphen;v) values for consistent component padding across the design system.  
**Dektop modes (medium and small).**  
  
**Token Group Space / wel / sem / spacingDynamic / insetSquish**:    
3xl-h: 48px  
3xl-v: 32px  
6xl-h: 96px  
6xl-v: 32px  
  
**Tablet and Mobile modes**  
  
**Token Group Space / wel / sem / spacingDynamic / insetSquish**:    
3xl-h: 48px  
3xl-v: 32px  
6xl-h: 96px  
6xl-v: 32px  
  
  
**InsetStretch**  
The `wel.sem.spacingDynamic.insetStretch` tokens provide responsive spacing values for non homogeneous padding elements &hyphen; resulting in a visually stretched layout. These tokens are defined as pairs of horizontal (&hyphen;h) and vertical (&hyphen;v) values for consistent component padding across the design system.  
**Dektop modes (medium and small).**  
  
**Token Group Space / wel / sem / spacingDynamic / insetStretch**:    
xl-h: 24px  
xl-v: 32px  
2xl-h: 32px  
2xl-v: 48px  
4xl-h: 48px  
4xl-v: 64px  
  
**Tablet and mobile modes**.  
  
**Token Group Space / wel / sem / spacingDynamic / insetStretch**:    
xl-h: 24px  
xl-v: 32px  
2xl-h: 32px  
2xl-v: 48px  
4xl-h: 48px  
4xl-v: 64px  
  
  
**PinchVertical**  
The `wel.sem.spacingDynamic.pinchVertical` tokens provide responsive padding values only on the vertical axis, creating a "pinched" appearance.  
**Dektop modes (medium and small).**  
  
**Token Group Space / wel / sem / spacingDynamic / pinchVertical**:    
xl: 24px  
2xl: 32px  
lg: 32px  
3xl: 40px  
4xl: 48px  
5xl: 64px  
  
**Tablet and mobile modes**.  
  
**Token Group Space / wel / sem / spacingDynamic / pinchVertical**:    
xl: 24px  
2xl: 32px  
lg: 32px  
3xl: 40px  
4xl: 48px  
5xl: 64px  
  
